# Journal

Corner Cursor

A portable trackball mouse

Started: 5/26/26

Current Hours: 33.3

## Day 1: May 26

Researched a lot about different configurations of trackball, and landed on a configuration that seemed suitable for the use it was meant for.
The main choice was between a thumb-controlled trackball and an index-controlled trackball. Ultimately ended up picking the index-controlled trackball because it was easier to use.
Also, it seemed that the position of the buttons would be more comfortable if the index finger were used instead of the thumb.

<img width="1472" height="798" alt="image" src="https://github.com/user-attachments/assets/747ba8a2-de7f-4bf1-95a8-9ec3ca3f73e6" />

Started fleshing out the basic equipment that would be required ot build a basic trackball, which would be useful to figure out the size of everything while
cadding.

<img width="2656" height="1630" alt="image" src="https://github.com/user-attachments/assets/70f8990f-44a4-4bf8-b68a-10b9adef701b" />

**Total Time: 2 hrs**

## Day 2: May 27

Mainly focused on the equipment that would be required to build the trackball, trying to get more specific with the equipment that would be used. This would help with the dimension that I would have to account for while trying to CAD. Turns out there are different forms of bearings for the trackball, but static bearings seemed the best. There are also different materials, but Zirconia Oxide seemed the most common. In terms of the sensor, Pixart has two primary ones that are in use. While the PMW-3360 is better, it is bigger compared to the PAW-3222.

<img width="2825" height="1568" alt="image" src="https://github.com/user-attachments/assets/9b03e89c-5d90-4c50-9825-f58767c73753" />

**Total Time: 1 hr**

## Day 3: May 28

Finished with most of the logistics of how everything was going to work, including how to track the motion of the scroll ring and what switches I would use for the buttons. I found a previous custom trackball with a scroll ring that used magnets and Hall effect sensors to track them, which seemed to work for my situation. The switches would be miniseithces made for mice from Omron.

<img width="2832" height="1574" alt="image" src="https://github.com/user-attachments/assets/7d0609fe-6495-4ba8-a7ad-30e5235fff86" />

Began CADding out the main case for the mouse, and with most of the materials figured out, I was able to know most of the logistics of what I had to do. I decided to put the trackball in the top right of the mouse and the two buttons next to each other in the bottom right corner.

<img width="879" height="616" alt="image" src="https://github.com/user-attachments/assets/c2499e4a-ae95-407b-ba57-9b29160e8b21" />

**Total Time: 2 hrs**

## Day 4: May 30

Worked out the logistics for CADing, primarily regarding the holder for the trackball. It turns out there are specific angles that can be used for the trackball. Originally, I was planning to use a 45-degree angle, but that seemed too steep, so I switched to a 60-degree angle, which was more relaxed.

<img width="2636" height="1586" alt="Screenshot 2026-06-12 161041" src="https://github.com/user-attachments/assets/86d194a8-a7ff-413a-88f4-f7597b1f6327" />

Finished with the design of most of the case, including the position and dimension of the buttons, and the basic design of the scroll ring was also being finished.

<img width="1060" height="1016" alt="Screenshot 2026-06-12 161718" src="https://github.com/user-attachments/assets/4260bc0e-ecdf-4459-82ce-ac307a8a61e6" />

Began with the holes to connect each part of the base, and making sure that there was still enough space for the PCB after the holes were completed. Also chamfered and filleted some of the corners of the CAD in order to make the case look more appealing.

<img width="1540" height="1256" alt="Screenshot 2026-06-12 162127" src="https://github.com/user-attachments/assets/8e4ac523-f0a9-4e24-8bd8-2a16f34b8376" />

Continued with making the holes in the case, to the point that I could fully assemble the full model in an assembly.

<img width="1232" height="1196" alt="image" src="https://github.com/user-attachments/assets/38573250-458b-44fe-8e04-d9c29062ae67" />


**Total Time: 4 hrs**

## Day 5: May 31

Worked on finishing up the pressing mechanism for the buttons so that I was actually able to mount them and use them to click the switches.

<img width="1430" height="1184" alt="image" src="https://github.com/user-attachments/assets/cd16e713-b47d-4e65-8bed-4fb8174a6fe0" />

Began on the schematic for the PCB. I originally intended to use the Seeed RP2040 as the microcontroller board because that is what I had used previously for a previous project with a keyboard. 

<img width="1728" height="1082" alt="image" src="https://github.com/user-attachments/assets/069b57ee-a4c2-479a-b38b-42e7ff0b8dbc" />

While doing a little more research, I found that maybe the Seeed board did not have enough ports, and I would probably just have to use the RP2040 chip in my design, which is a lot more complicated because it needed many more things rather than just hooking up components to each other. I was going to save that for the next session, though.

<img width="2620" height="1554" alt="image" src="https://github.com/user-attachments/assets/e4e2c13e-06a7-454e-a66b-af8e9dd363f2" />

**Total Time: 3 hrs**

## Day 6: June 2

I had my second thoughts about using the Hall Effect sensor, which was whether it was really the best way to track the movement of the scroll ring. My doubts stemmed from my lack of knowledge of how they worked and how to wire them in KiCAd. However, after doing more research about the other methods of how to (mechanical & optical), it seemed that the Hall Effect sensor was the way to go.

**Total Time: 0.3 hrs**

## Day 7: June 4

The day of reckoning came when I had to deal with how to use the RP2040 on its own. I thought I would be cooked because there were a lot of pins, but I ended up just using the hardware handbook thing that they recommended in order to get the basic stuff down. It seemed my worries were not valid.

<img width="2536" height="1348" alt="image" src="https://github.com/user-attachments/assets/4094a0c1-97a4-4e99-bb56-1385bc15be2e" />

I began feeling more comfortable as I got the symbols for the switches and the flash memory as well as the crystal that would serve as a timer. The hardware sheet that Raspberry provides is very useful because it provides basically all of the example schematics, which I can cross-reference with custom trackballs already on git.

<img width="2536" height="1348" alt="Screenshot 2026-06-12 164716" src="https://github.com/user-attachments/assets/f6eaee1b-1c1b-44a7-aa6e-d6127ac4a2cf" />

Using the datasheet, I began wiring up the capacitors and the resistors for the separate components. I've finished the wiring for the sensor for the trackball.

<img width="1750" height="1188" alt="image" src="https://github.com/user-attachments/assets/c0f571b7-efe8-4603-8782-6ef30f67f742" />

**Total Time: 3 hrs**

## Day 8: June 5

I finished up a lot of the PCB schematic in KiCad that was left. More specifically, for the crystal, USB, flash, and switches, I did the capacitances as well as the resistance.

<img width="1934" height="1252" alt="image" src="https://github.com/user-attachments/assets/4e5e270c-6771-4a6d-b398-17761b4f3e3f" />

**Total Time: 1.5 hrs**

## Day 9: June 12

I switched over to Horizons from Fallout today.  In order to make this project shippable to get my hours, I had to properly document everything in GitHub. So, I spent most of my time writing the journal for the repo and setting up other things.

<img width="2914" height="1770" alt="image" src="https://github.com/user-attachments/assets/392ea77b-d231-42d0-99a4-c588ee9207c5" />

With most of the GitHub stuff done, I began to finish the schematic on KiCad. I pretty quickly did all of the connections for the remaining stuff, which was the decoupling capacitors on the RP2040 and the power supply. However, I did manage to finish the schematic, and unfortunately would have to fix all the problems in the ERC now.

<img width="2200" height="1322" alt="image" src="https://github.com/user-attachments/assets/f3431b63-ecc5-4e96-9d16-95a7aaf99143" />

**Total Time: 3.3 hrs**

## Day 10: June 15

I began by verifying all of the connections that I had made previously, as I had kind of been rushing. I fixed the errors, and I was off to assigning footprints to all the symbols. I imported many of the footprints, which was kind of confusing because the imported ones were not showing up. However, eventually, I got it to work. I also found out the different sizes for capacitors and resistors.

<img width="2944" height="1730" alt="image" src="https://github.com/user-attachments/assets/fe22b8ce-57fc-459e-9064-02dcc5c48edf" />

After finishing off the footprint assignments, it was time to fix the rest of the problems with the ERC. Most of the warnings were simple to fix because they had to do with having to fix wires or edit symbols so that they fit properly. However, there was one error and warning that was evading me, which had something to do with a GND pin and a +3v3 pin. As much as I tried to figure out what the problem was, I could not fix it, so I just moved on to the PCB editor, hoping that it would not cause any problems.

<img width="2222" height="1312" alt="image" src="https://github.com/user-attachments/assets/c7a1f971-b8c9-4e24-9a1e-5aa15dbf86a0" />

I imported all of the footprints into the PCB editor and laid out all the components properly. I used my CAD model in order to accurately replicate the usable dimensions for the board. Although it seemed that I would not have enough space, in the end, it turned out that there was space.

<img width="2176" height="1328" alt="image" src="https://github.com/user-attachments/assets/3750fad7-a6d8-4a6b-9663-e157f2d10e21" />

From this point onward, it seemed kind of weird. From my past experiences, I knew that while traces were a tedious process, it was pretty straightforward about what you needed to connect. However, in this instance, it seemed that ratsnests were leading me to wire the wrong components together. For instance, it wanted me to wire the pads of the capacitor together, which did not seem correct. I even looked at some video tutorials, but I still didn't seem to be able to wire the correct pads.

<img width="2180" height="1322" alt="image" src="https://github.com/user-attachments/assets/e27f0ad1-72bb-4345-bb76-bff57b86f355" />

**Total Time: 7.5 hrs**

## Day 11: June 16

Started with fixing the big problem that was bugging me before, which was the reason why previously I couldn't begin tracing. It turns out that the line of decoupling capacitors connected to the RP2040 had been wired incorrectly, which resulted in all of the GND nets turning into +3v3 nets. With that out of the way, I could begin successfully wiring the PCB, and it was pretty easy in the beginning.

<img width="1708" height="948" alt="image" src="https://github.com/user-attachments/assets/f4cc0b9a-6086-4b95-ad36-48516ce57e61" />

Now the more challenging wiring came, and it was really hard. I had to use a lot of vias on order for the traces not to cut off each other. In hindsight, I should have thought about positioning the components on the board so that it would be easier for me to wire. For the first time, I used different sizes of traces so that I could make power lines thicker than signal ones.

<img width="2942" height="1780" alt="image" src="https://github.com/user-attachments/assets/e32d706d-f583-4039-aec8-e55465fb68b8" />


**Total Time: 4.5 hrs**

## Day 12: June 16

Fixed up the remaining problem with the DRC in KiCad. The majority of the issues just came from small bits of traces being left out, and silkscreen making things problematic.

<img width="2912" height="1670" alt="image" src="https://github.com/user-attachments/assets/5f1f7a06-e94c-4d5c-9a5d-079a944141eb" />

Used the code from a similar project to get the firmware working. It was pretty simple, as I only had to adjust some PINs. I did not realize, though, that on RP2040s, there are specific pins for the SPI protocol that are divided into different SPI blocks. This made me have to rewire some stuff, but in the end, it was not too much work. I finished up the repo today as well.

**Total Time: 1.5 hrs**




