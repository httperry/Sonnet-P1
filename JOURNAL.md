---
title: "Sonnet P1"
author: "httperry"
description: "A UWB and mmWave based Hand Gesture Recognition device aimed to help translate sign language and gesture recognition for VR applications"
created_at: "2026-08-25"
---

# 2026-09-07: Started 3D Modelling for the Enclosure

**Total time spent: 6 hours**

[Part of the Database incidence and migrated to this new project from the [old](https://forge.hackclub.com/projects/1857) one]

Halo!

So firstly I'll explain the project cause I dedicated my time today towards research and starting the 3D model work, and started with the bottom shell today. The project is based on Google's Research named Soli which uses a 60GHz based mmWave FMCW Antenna-In-Package (AIP) chip to track hand gestures. This was implemented in the Google's Pixel 4 too

My approach is to use a 60GHz FMCW to track hand gestures with greater precision and also use UWB based tracking to get an estimated position of the hands too. I plan to use the 3D point clous to create a hand skeleton using python libraries, I will create a framework that converts the data that it recieves as input from the antennas into a 3D Vector ig? (Still working on that) and then I can use those gestures in different ways, currently I can only think of using it for Sign Language Translation and in VR/AR applications :cry-ok:

For the Sign Language translation I am going to use a pre-built machine learning model trained to translate sign language to normal english using 3D vectors (Not confirmed) and use TTS to speak it out through the speakers, I am thinking of using [Sarvam AI](https://www.sarvam.ai/) to translate it to other languages live. The sign language to english translation will be on-device but for better features I will offload the work to other providers. I am also making the project with privacy in mind as this will be way better than using a camera as through this it doesn't breach the privacy and exposure to camera of the other person u are talking with just for the sake of communicating, also I am going to add a privacy kill switch that turns off the access of the device to internet via WiFi or Bluetooth at a hardware level. As for the application in AR/VR fields, I am going to create drivers for these that I can use to connect the device to the PC via bluetooth or wifi and provide the gestures directly to games or expose it via an API for developers to continue developing for this and creating apps

That being said, today I started my work on the 3D Model of the enclosure, I am taking inspiration from the [Nothing CMF Buds Pro 2](https://in.nothing.tech/products/cmf-buds-pro-2?Colour=Orange) which is a slim and squarish form factor of earbuds, so I am making the device 60x60x20mm out of aluminium CNC so that it is rigid and sturdy (Yes I had to use CNC as the form factor is going too small and it was becoming too hard for it to be 3D printed and this was my first technical CAD) and I created the bottom shell body

![image](https://cdn.hackclub.com/01a11a8f-6ec7-78b3-a7c6-a072c2d8dfac/Screenshot%202026-10-08%20133703.png)

**Kindly note that I have tried to recover the screenshot from the lapse as I don't have the old screenshots with me anymore**

That's it for today

Adios!

# 2026-09-08: Worked on Hinge Design in CAD

**Total time spent: 4.5 hours**

[Part of the Database incidence and migrated to this new project from the [old](https://forge.hackclub.com/projects/1857) one]

Halo!

So today I worked on the hinge and I have worked on the hinge which was by far the most hardest thing I've done (actually I have worked on the same hinge 3x for forge but then I forgot to lapse it and now after so much research it seems lik 4hrs :ok-cry:)

I first thought of using a knucklehead design but then I had to find a way to route the battery wires from the bottom shell to the topshell and it was such a pain to do :despair:, I first thought of how laptops used to do this and they used a through axle method where the passed the wires within the hinge but I am not a master of than and the sizes were too small too like the axle was 2mm! so then I thought of using an around the hinge approach where the wires wouldd go around the hinge instead of through it and it worked flawlessly! Kinda I then had to figure out the appropriate point of roation and radius of rotation and ensure nothing collides, there are still a few works remaining on it but that's it for the day. I also worked on adding a channel to route the wires through

![image](https://cdn.hackclub.com/01a11a98-c3d3-7903-816c-427816c6ef39/Screenshot%202026-10-08%20134915.png)

**Kindly note that I have tried to recover the screenshot from the lapse as I don't have the old screenshots with me anymore**

I will be continuing the work on the hinge and finishing it off today or tomorrow

Adios!

# 2026-09-09: Completed Hinge Design in CAD & Created Notch in front

**Total time spent: 4 hours**

[Part of the Database incidence and migrated to this new project from the [old](https://forge.hackclub.com/projects/1857) one]

Yallo!

So today I finished off the hinge design and the only thing remaining rn is the top shell, before moving on I noticed a notch on the bottom half of my mac which gave me an idea to create a similar notch on my enclosure for ease of opening and closing 

So first I thought of creating a simple extrude in a different plane and moving the edge down to create a plane there for the finger to slide on and then use fillet to round off the sides, but Fusion had it's own mind and didn't let me do that so then I had to keep trying different tools that'll allow me to create the wedge I want, finally loft was the one that worked for me. I created the sketch and then used loft to create the smooth surface I was looking for and finished off the notch

![image](https://cdn.hackclub.com/01a152d7-bed4-7069-9535-63c5447748e4/Screenshot%202026-10-19%20115630.png)

![Screenshot_2026-09-12_at_10.57.39_PM.png](https://cdn.hackclub.com/01a0a112-a2c3-79b2-b3c1-5d2c91d45aef/Screenshot_2026-09-12_at_10.57.39_PM.png)

**Kindly note that I have tried to recover the screenshot from the lapse as I don't have the old screenshots with me anymore**

That's it for today!

Adios

# 2026-09-12: Finished CAD modelling of Bottom Shell (Nearly)

**Total time spent: 2.5 hours**

[Part of the Database incidence and migrated to this new project from the [old](https://forge.hackclub.com/projects/1857) one]

Yallo!

So today I finished most of the work on the Bottom Shell!! The issue I was facing that when closed and open there was enough clearance between the top and bottom shells, but while opening both were colliding :pain:

So I tried to increase the spaces between them but then got to see a massive gap in between the shells, then I took inspiration from my mac where there is a rubber gasket or ring around the edge, which in addition also helps in reducing the snapping noise created, for that I created a channel to add the gasket later. I'll be moving onto the top shell next

![image](https://cdn.hackclub.com/01a15310-26ac-771c-bacd-c313fd6bc758/Screenshot%202026-10-19%20125840.png)

**Kindly note that I have tried to recover the screenshot from the lapse as I don't have the old screenshots with me anymore**

That's it for today

Adios

# 2026-09-13: Worked on Github Repository [Work done by npc.jdp]

**Total time spent: 4.5 hours**

Okayy Hello world, this is my first time entering a journal for this project, and I worked for 4 hours straight, simple stuff, just worked on the read me md files, since it was my first time using hackatime, it took me a while and a few fails, so I decided to code on github's code space.

here is the github link for reference ( https://github.com/httperry/Sonnet-P1 )

here is my split of time for the same:

2 hours - Research on how to use git(commit/push allat) + took inspiration on how to structure the repo files from httperry's previous repos and aligned it with our current repo

2 hours - Coding the whole repo's backbone (all the folders and every folder's own readme file)

30 minutes - figuring out out to set up hackatime, I actually tried using lookout, but realized I'm not allowed to, and ironically there was a bug on forge that didn't allow me to add my hackatime project to the project as a collaborator, i'll connect it later when fixed. 

that's it from my side for today 

Here are the images for the same:
![image.png](https://cdn.hackclub.com/01a09a2a-fd65-7bd1-a165-5b2ba14c8dd0/image.png)
![image.png](https://cdn.hackclub.com/01a09a2b-17e7-7a27-a099-87f4ef53d34e/image.png)
![image.png](https://cdn.hackclub.com/01a09a2b-2a34-78b9-8661-b9374a777513/image.png)

# 2026-09-15: Finished with Bottom Shell in CAD Design

**Total time spent: 4 hours**

[Part of the Database incidence and migrated to this new project from the [old](https://forge.hackclub.com/projects/1857) one]

Yallo!

So today I went on amaon to do dig deep in a rabbit hole of sealants and gaskets, first I was thinking of using a gasket but there wasn't enough space, then I though of 3D printing the gasket but it will break sooner than expected. Then I discovered Silicon Sealants which like u paste it like glue, leave it for a day or so and it hardens into bendable rubber

So for that I chose to use `Feviseal Neutral Pro` (I swear I'm not brand promoting) which is a great sealant and is pretty cheap, then I thought of filling the channels with the sealant and then using a tool to scrape the excess and leaving behind a wedge of silicon, but it was difficult to scrape that by hand perfectly. Then I went ahead to design a lid that I can place on top and squeeze to remove out excess sealant like working with clay 

![image](https://cdn.hackclub.com/01a15333-5f5a-7b89-83e5-d21a793e7b79/Screenshot%202026-10-19%20133702.png)

**Kindly note that I have tried to recover the screenshot from the lapse as I don't have the old screenshots with me anymore**

I then moved onto thinking on how I will add the axle in the middle of the hinge, then in the CAD I thought of creating a channel for the axle so that I can insert it at an angle but that was a huge pain to model in CAD and isn't feasiable based on manufacturability, then I thought of using spring loaded watch pins and found the perfect size one at [cousinsuk.com](cousinsuk.com) and added it to cart :oke:

That's it for today!

Adios!

# 2026-09-17: Started working on TopShell and limted the movement of the topshell near the hinge

**Total time spent: 2 hours**

[Part of the Database incidence and migrated to this new project from the [old](https://forge.hackclub.com/projects/1857) one]

Yallo!

So today is an important day, where I mark the top shell as finished and mark the CAD modelling as done! So today I modified the topshell to add sections and lips (1mm ledges) for the polycarbonate sheet that will go in the front and also the mounting holes for the PCB

I then moved onto the top shell hinge in which I thought of ways to limit the movement of the topshell, I extruded a wedge out of the top shell knuckle and created a channel for it in the bottom shell which prevents further movement of the top shell

This was way simpler than what I imagined on how complex it will be

![image](https://cdn.hackclub.com/01a1535e-4d4b-7810-8a99-0690bd3a5fd8/Screenshot%202026-10-19%20142354.png)
![image](https://cdn.hackclub.com/01a1535e-4df3-7013-8b0e-4593aa040ef0/Screenshot%202026-10-19%20142343.png)
![image](https://cdn.hackclub.com/01a1535e-4efa-7824-8962-a101788de71d/Screenshot%202026-10-19%20142326.png)
![image](https://cdn.hackclub.com/01a1535e-4fc6-7342-89c4-031fb1305a1c/Screenshot%202026-10-19%20142206.png)

**Kindly note that I have tried to recover the screenshot from the lapse as I don't have the old screenshots with me anymore**

That's it for today!

Adios!

# 2026-09-17: Created Cover Image and Logo assets for the Project

**Total time spent: 0.75 hours**

Halo!
So since my last journal entry I have finished creating the cover image design in Canva and the Logo in MacOS 27 Icon Composer :yay:

Here’s how they look:

![Sonnet_P1.png](https://cdn.hackclub.com/01a0ae2e-edf2-7905-87c9-3b95e54b6b9b/Sonnet_P1.png)
![Sonnet_P1-macOS-Dark-1024_1x.png](https://cdn.hackclub.com/01a0ae2f-70ac-76b8-b3b7-fd8734eaf9d9/Sonnet_P1-macOS-Dark-1024_1x.png)
![Sonnet_P1-macOS-Default-1024_1x.png](https://cdn.hackclub.com/01a0ae2f-6b2e-7539-92d0-1c610226bae5/Sonnet_P1-macOS-Default-1024_1x.png)

That’s it for now, I’ll continue further to finish up the top shell CAD and mark it as finished for good

Adíos!

# 2026-10-19: Moved old journals from previous project and recovered deleted journals due to the database mishap

**Total time spent: 6 hours**

Yallo!

So it took me quite some time to shift all the journals from the previous project to the new one, with the burden on top of recovering the old deleted journals due to the database mishap, but I have successfully managed to shift all the journals and shifted the journals to my github repo incase this happens again (which I hope doesn't happen :prayer:), the reason I had to create a new project was because I was instructed by the Fraud Squad to do so and verified that I can submit this project with them (if you still think this isn't allowed plz DM me first and we can discuss this further on slack)

But at last all the journals are updated and completed with proper descriptions of the work done, I have updated the GitHub for this too

That's it for today!

Adios!
