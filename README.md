# Ryzentosh-5900hx-mofire-s500
 -Anything impossible hardware are used in this little cube. And the goal is to make it same as Apple's\
 -If you like this project and want to download the EFI, please let me know \
**Hardware**:
- cpu:5900hx-es
- gpu:vega8-es
- network:realtek
- wireless:-wifislot bcm94360ng(airdrop) ax210 200 (test)
- motherboard:demo board (lookup amd b550 motherboard)
- others:two m.2 slot. 2xusb3.0 4xusb2.0 1xDP 1xHDMI; Monitor using dp-direct-connetted b160qan02.q
- newbought: rx6600xt some acpi and changes in device tab
           \
**OS**:
- MacOS Ventura(tested 13.3-13.5.1) Sonoma14.1(with Opencore lagacy installer)
- OpenCore 0.9.0 & 0.9.3

 # Progress:
 - all things worked so as airdrop.
 - Fixed wifi slot dsdt issues so wifi is finally working (took me 2 months to figure it out) 
 - monitor enabled hidpi and 165hz with hidpi.sh
 - Trying to fix ramdom system-inresponse or rebooting issues for several months
 - Tryied newest Os,that is Sonoma, install on a different apfs volume. I managend to get all things worked
 # Knowing issues:
  - can't use pbo for amd cpu as it can crash down the os. This is a mess for my work.\
    fix：only needs to disable curve optimize in bios setting, others like power limits, maxoverclock speed and ratio can set as high as your board can
    Be careful about the heat dissipation. Say the edge-high performance is highly power demanding.so maybe a more miled setting can prevent you from throttling very soon.
  - operating sys encounter black screen sometimes when booting up\
    For months of using this hackintosh, I have not figure out the reason.
  - system sometimes stuck and must force to reboot and throws panic.(Thought to be nootred issues while no hardware failure in panelty test)\
    fix1: also PBO or--the mini pc only have a positive fan for cpu cooling so that the memory cooling is not enough with just passive cooling.You should try adding some stuff to cool the memory. (My way to fix is add a some thermal conductivities to transfur the heat to the metal shell and a small-low-rpm-no-noise-side fan will bring the heat away!)
    fix2: (constucting)cpu watchdog switch to "no error",and internal time 21s. The hackintosh can run about half a month with no acidental rebooting.
  - power bottom can not function
    no fix for now
 # Update of Knowing Issues
 - Audio DAW may stop playback or have cracle sound as there are some wierd trap of the cpu, even the load of the audio chain is pretty simple
   Fix: after testing for a day, the issue is the wifi. Maybe the wifi search and reconnect action causes lock of the cpu. So the fix for now is to turn the wifi down in the system setting(you shell see a strip through the wifi logo). And if you're not a audio engerneer like me, you can ignore this fix. Maybe there are other ways,but just be sure there're noting wrong with your work flow:)
