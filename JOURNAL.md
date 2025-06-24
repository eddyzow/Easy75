---
title: "Easy75"
author: "Eddy Zhao (@eddyzow)"
description: "A custom, feature-rich 75% gasket-mounted mechanical keyboard run with a Raspberry Pi Pico."
created_at: "2025-05-24"
---

*Total hours spent: 53* | *Date started: 24 May 2025*

# Easy75
_because sometimes nine keys isn't enough..._

## entry #14 - 6/23

and with that, the Easy75 project is now complete!

some final pictures and a sound test:

[Easy75 Sound Test - Stock Akko V3 Creamy Blue Pro, Stock Durock V3](https://youtu.be/ZoHuPwVao3s)

![image](https://github.com/user-attachments/assets/ff1d0397-0a16-4dc5-a085-193459c8a53c)
![image](https://github.com/user-attachments/assets/787cace3-3fe4-442a-87d7-bcea9cb0c205)
![image](https://github.com/user-attachments/assets/e822f602-3317-46e8-b09b-49cc46fb0e5d)
![image](https://github.com/user-attachments/assets/e473a912-7f04-4c1a-a078-2a01bf1f2be6)
![image](https://github.com/user-attachments/assets/faa09bd5-c77b-43a7-9b6b-1634680ae53c)
![image](https://github.com/user-attachments/assets/6c45d9ef-dceb-40ed-9566-c7855e604e2d)
![image](https://github.com/user-attachments/assets/01b22a00-8f02-4b77-b1d3-81aa750fa440)


although I bet nobody will read this, if you are, thanks for looking at my engineering design process. i hope that i'll learn how to engineer better stuff in college.

## entry #13 - 6/21

it's been a grueling last two days. i've spent so so many hours trying to make this work, but i keep making terrible mistakes along the way. I soldered the raspberry pi pico on backwards after taking three hours to solder all the diodes and kailh sockets. the plate isn't strong enough and the switches are weakly housed in the sockets. furthermore, I then had to dremel the incorrectly soldered pico off the PCB because there was no possible way to desolder (even with a solder sucker). 

I finally finished putting the electronics together today. somehow the raspberry pi pico was not completely destroyed and i was able to load my code onto it. however, errors upon errors continued due to many of the pins being completely killed by my reverse soldering. the I2C from the board didn't find the OLED screen because the connection was too weak and there were no pull-up resistors (i thought these were part of the screen). the rotary encoder wouldn't work no matter what i tried. and when plugged in, the keyboard would randomly send inputs for random keys, with ghosting like crazy -- even though i had soldered 84 diodes to avoid this. typing one key would cause an entire column to be inputted, and some keys didn't work at all. here's a screenshot of the working key map for the board:

![image](https://github.com/user-attachments/assets/39f514c6-8c63-465a-82d2-6095e9e9b99e)

as you can see, not many of the keys work. 

i would really have loved to type this journal entry on my new keyboard, but i'm out of budget. i've spent so much extra money out of pocket on this project and I am tired and want to give up.

but I shouldn't give up! i had two goals when i started this project: to create a work of art that sounds amazing, and also to create a functional keyboard. while one of those goals is no longer possible, the other is completely up for grabs and the functionality doesn't change the fact that it does sound great. i will be making a video of the project when i finish and submit it. even though it doesn't work, it was still a great first try at making a board, and i learned a lot! and i'm sure the next time i will make a keyboard, i'll be able to get it right... granted i don't reverse solder the microcontroller.

![image](https://github.com/user-attachments/assets/05f295ff-6c53-482c-8eb0-23d680a32cb5)

_hours spent during session: about 12 hours_

## entry #12 - 6/13

i've finally fixed Easy75 to not have RGB! and as another cost-cutting measure, i'm going to 3D print my switch plate. it shouldn't be too bad lol

![image](https://github.com/user-attachments/assets/00811934-add2-4e59-8ef4-7c931a5645b2)

also, all the parts are now fully purchased. and i'll return the LEDs i don't need anymore.

thanks to a godly blessing (alex ren) JLCPCB is actually $30 cheaper than i had expected!! and thus i only needed to pay $37 to JLC for my PCB instead of $180 to PCBWay (sheesh man!!) 

(approx. 4hr spent in this session)

## entry #11 - 6/12

it's been a week and a very hectic one at that. I graduated high school! and now I have some bad news to share about Easy75.

I'm getting rid of the RGB to cut costs -- this cost a significant amount of the project and I also don't have the experience nor time to put it together. 

the PCB costs are way higher than I had initially expected -- both JLC and PCBWay had given me lower costs initially upfront and that is what I had put into the BOM. however, upon hitting checkout, they surprised me with a bunch of extra costs, increased shipping fees, and tariffs which i had initially expected to be part of the board cost.

thus, i've had to make this difficult decision -- but i hope that easy75 will still be a big success! 

## entry #10 - 6/5

after review, the case is too simple to be accepted as a highway project... so I redesigned the whole thing!

introducing Easy75 v2, which is even crazier than ever!

the keyboard is now gasket mounted. i did this by layering some rubber gasket material around the outside of the bottom case. by screwing the plate into the case, it must sit on top of this gasket material. this should do wonders for the keyboard's sound profile!

i also added a 4.5 degree incline for ergonomics... and the case is no longer just a box!

as a result i've had to cad a separate top case for the keyboard.. but that's not a big problem! 

![image](https://github.com/user-attachments/assets/a9200213-6cd7-4519-a274-331ab063d7d4) (the board!)

![image](https://github.com/user-attachments/assets/95a1883b-138b-4d07-93f7-aaa001da81fc) (gasket strips -- there will actually be more but I added a short strip in the CAD for clearance purposes)

and now I can finally say it's done. looking forward to getting the parts and putting this baby together!!

(approx. 3hr spent in this session)

## entry #9 - 6/1

Easy75 is done being designed!!

the firmware honestly was not hard at all to code -- i just copied what i had from my macropad (ezpad) and extrapolated it to fit my new 84-key grid. i've attached it to the repository. and now i will be submitting this for review. once i get my grant i'll go purchase the parts and put it together!

## entry #8 - 6/1

the hardware is officially done!!

![image](https://github.com/user-attachments/assets/4c3bdbb5-bbd6-4dec-8a9b-db7a4c616352)

mounting holes are added. the firmware shouldn't be too bad to code -- once it's done i will submit to get my grant to build! i'd like to explore how i can get jlcpcb to solder some of the components because i am NOT at all confident in my soldering ability especially when soldering is quite painstaking and i would have to solder multiple wires for each switch... hundreds of connections. i will, however, have to solder the surface-mount LEDs manually. 

also, i got rid of the sloped angle because it's hard to machine and it got in the way of the mounting holes. i might make something later for ergonomics

## entry #7 - 6/1

happy june! i've realized i made a huge mistake when i have no mounting holes in my PCB. turns out that the guy who made the footprint and symbol pack i used (scottokeebs) uses plate mounted stabilizers... but the plate-building tool i used clearly does not support plate mounted stabilizers and assumes that i am using PCB-mounted stabilizers. i had to go back and search across the internet to find out where the pcb mounting holes were supposed to go. i felt really stupid at the end because i discovered that you didn't actually need to place footprints by attaching them to schematic symbols but you could actually just place them directly on the PCB. and lo and behold, scottokeebs had a set of footprints with stabilizer holes that i didn't see earlier. this took SO LONG!!! not to mention that i had many many MANY wires running through the area where the mounting holes are, and i had to reroute them all.

but finally I think I'll be able to submit soon! just figuring out mounting holes and then firmware. i also downgraded the board from gasket-mount to a normal top plate mount since the whole point is that it is an "easy" first board. a future board will be gasket-mount. also currently there is no "secure" connection between the plate and the pcb except the switches -- i need to get this mounted as well. but that's something for tomorrow!

![image](https://github.com/user-attachments/assets/e3728ead-758a-4dce-87b3-459839278b3c)

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




