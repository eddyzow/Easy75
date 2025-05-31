*Total hours spent: 26* | *Date started: 24 May 2025*

---
# Easy75
_because sometimes nine keys isn't enough..._

## entry #6 - 5/31

i've finished everything on the hardware end for this small but also big project! i did have some strange problems on onshape as my document completely broke -- it stopped loading when i tried to change an appearance and even after reverting it wouldn't load anymore. so I had to export each individual part, copy to a new document, and delete the old document. i am now uploading all the hardware parts to this repo. it's 3:58 am while i'm typing this and i think i'll go to sleep once i finish writing at least some of the firmware (something is wrong with me).

## entry #5 - 5/31

it's been a busy few days -- today was my last ever day of high school!! and even amongst the bittersweet goodbyes and yearbook signings ahead of an even busier graduation week lies my work on Easy75!

![image](https://github.com/user-attachments/assets/86acc884-ac14-4f03-9f6a-c18b4971caca)

I spent the day creating the PCB plate in CAD, which must be 1.5 mm thick. I will use pololu's laser cutting service to get this machined. this plate neatly fits into the case, holds the switches, and provides a snug typing sound while separating the electronics from my grubby fingers. i used ai03's plate generator and keyboard-layout-editor.com to generate the DXF file for the keyboard layout. I really, really, REALLY am starting to love how this is looking. And I think I'm working so fast that I might be able to get this produced and built in less than a month!

and the final result looks like it might be coming to fruition... look at the image above!

## entry #4 - 5/29

![image](https://github.com/user-attachments/assets/5c2c175e-1ec1-4b73-94ab-76c796776c98)

as soon as i got home i got to work on onshape -- much work has been done on the CAD. i've created the main board (which should be cast in resin) and have the pcb being mounted on rubber gasket strips. i now need to create the plate, which must have the proper stabilizer holes to work properly. i'm really happy with where this is going and if i spend a little more time i'll have a solid design that i can get shipped off. i've decided to use pololu's laser cutting service to get an acetal switch plate machined -- hopefully this acts similarly to polycarbonate and delivers the THOCK typing sound we all love.

## entry #3 - 5/28
PCB WIRED UP!!

after a buttload of painstaking work that took multiple hours, the pcb is wired up! all that's left is to create holes for stabilizers, CAD the case, and ship! here's a pic of the final design (i am quite bad at wiring so yes it is a little messy):

![image](https://github.com/user-attachments/assets/d581f00b-c179-4b09-851a-0e7dfb78bde2)

i really really really hope the finished product will work. this is going to involve tons and tons of soldering, and i've also never soldered more than just a few chips for my old robots -- this is taking it to the next level...

i'm also deciding on what switches/keycaps/stabs will be used. in order to save hack club's precious dollars i will use akko creamy blue pro v3 switches ($0.29 per switch) -- in the past i have had an excellent experience with akko switches as they are super cheap and ridiculously good sounding for the price. for stabs i'll use durock v3 and for keycaps i will try to find a solution but since i want this keyboard to be the very best i may splurge and get a set of GMKs on my own budget. i think i will cast my case out of resin with a 3d printed (?) mold or use acrylic. 

## entry #2 - 5/27
PCB ORGANIZED??
here is what it looks like, with all the LEDs added, parts positioned, and about 20% done with wiring:

![image](https://github.com/user-attachments/assets/055a1d67-13d2-45a8-9196-b8b68c250b7c)

i'm still not fully sure what i actually have to solder vs what jlcpcb will do... hopefully i don't receive the pcb and then realize i don't have the necessary parts!!! i think from my current knowledge i have to solder the diodes and the switch sockets
also i don't know where stabilizers go on the pcb yet... i'll figure this out with some research. for now the pcb is doing just fine!

also, the wiring is going to be hell but i'll get through it. i have 516 paths i have to route 💀

## entry #1 - 5/26

i'm back from vacation! as soon as i got home i got to work creating the first version of easy75. i was able to get the entire schematic and some of the pcb done. here's a preview:

![image](https://github.com/user-attachments/assets/07605ee6-8bb7-4876-873f-9fc336de4ca1)
![image](https://github.com/user-attachments/assets/1a22989f-98cb-47cc-a8b6-45e8b32fa0da)

the keyboard is powered by a raspberry pi pico. if i can get my hands on a pico 2 then i'll use that. because i had the OLED screen and needed space to put the MCU, i had to add the extra six keys a little strangely leaving some space, but i think it'll be okay in the end.

when i made hackpad, i found that the hardest part was wiring and adding the LEDs. i haven't done that yet so wish me luck as i navigate this once again!!


## introduction (entry #0 - 5/24)

welcome to my journal for my **THIRD** hack club highway project! this is a custom-designed and built 75% keyboard. the name comes from both my initials (EZ) and the overarching principle that this keyboard should be easy to build. last week I built a macropad from scratch, opening my eyes to the world of custom keyboard PCBs. i want this to be a step up from a macropad but not at the level where I'm hiding the MCU under the spacebar on the reverse side (though i do wish to reach that point someday).

some features i wish to incorporate for this project:
- hotswap
- gasket mount
- per-key RGB
- 1.3" OLED screen (128x64)
- custom firmware that would support n-key rollover
- rotary encoder(s?)
- custom PCB
- lubed switches/stabilizers
- more!

i will use KiCad for designing the schematic and pcb and Onshape to CAD everything. machining the case will be difficult but i will attempt to create something that works out given my limited 3D printer space. maybe i'll even be able to get access to my robotics team's CNC machine. for now, we shall begin designing soon. first i have to go on vacation for a few days...




