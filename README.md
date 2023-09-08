# Ryzentosh-5900hx-mofire-s500
-anything impossible hardware are used in this little cube. And the goal is to make it same as apple's \
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
  - operating sys encounter black screen sometimes when booting up
  - system sometimes stuck and must force to reboot and threw panic.(predicted to be nootred issues while no hardware failure in panelty test)
  - power bottom can not function
