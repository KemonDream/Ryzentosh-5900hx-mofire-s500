# Ryzentosh-5900hx-mofire-s500
-Anything impossible hardware are used in this little cube. And the goal is to make it same as Apple's
- If you like this project and want to download the EFI, please let me know \
**Hardware**:
- cpu:5900hx-es
- gpu:vega8-es
- ethernet:realtek
- wireless:ax210 200 bcm94360(for test)
- motherboard:demo board
- others:two m.2 slot. 2xusb3.0 4xusb2.0 1xdp 1xhdmi; monitor using dp direct conneted b160qan02.q \
**OS**:
- MacOS13.4.1 Ventura
- OpenCore 0.9.0 & 0.9.3

 # Progress:
 - all things worked so as airdrop.
 - Fixed wifi slot dsdt issues so wifi is finally working (took me 2 months to figure it out) 
 - monitor enabled hidpi and 165hz with hidpi.sh
 # Knowing issues:
  - can't use pbo for amd cpu as it can crash down the os. This is a mess for my work.
    fix：disable curve optimize in bios setting
  - operating sys encounter black screen sometimes when booting up
    fix: also related PBO, method same as above 
  - system sometimes stuck and must force to reboot and threw panic.(predicted to be nootred issues while no hardware failure in panelty test)
    fix: also PBO or--the mini pc only have a positive fan for cpu cooling so that the memory cooling is not enough with just passive cooling.You should try adding some stuff to cool the memory. (My way to fix is add a some thermal conductivities to transfur the heat to the metal shell and a small-low-rpm-no-noise-side-blowing fan will bring heat away!)
  - power bottom can not function
