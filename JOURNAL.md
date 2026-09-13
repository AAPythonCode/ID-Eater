# Journals
Hey! I'm Ayaan, a 13 year-old who's spent ~1.5 years on Hack Club! This is where I'll post all of my journals, specifically made for the program [Gadget Market](https://gadget.hackclub.com).

## 8/25/26
### A Summary Of What I Did Today
Today, I didn't build or CAD anything! Instead, I focused primarily on designing the Bathroom Pass using [Web Whiteboard](https://webwhiteboard.com)!
The diagram includes the wiring diagram, the links to all of the parts via AliExpress, and a small CAD diagram showcasing some useful images of the to-be CAD. 
I've tried to be as accurate as possible with the wiring, even color-coding the wires and creating pins to connect them to!

### Researching
After about 20 minutes of researching, I found three very important parts: 
- A barcode scanning module (without the traditional external handle and button configuration, EVAWGIB DP08)
- An ESP32-C3 (which had all the necessary pins and antennas, thankfully including WiFi and Bluetooth)
- A 360 degree servo (EMAX ES08-MD)

The barcode scanner would scan the barcode on the ID and lower the ID while the person went to the bathroom, while the ESP32-C3 would emulate a keyboard (using Bluetooth) to give the person a hall pass (using the 5starstudents software).
Then, once the person came back, they would click a button, which would emulate a keyboard to check the person out and simultaneously give the ID back to the person!

I also had to go through various data sheets and diagrams to figure out how to wire all of the components together!

### Problems And Tedious Tasks
Wow, I sincerely wish this section didn't exist! However, we all encounter these in some parts of our designing process.

Firstly, one of the major tedious tasks of the building process was finding all of the parts on AliExpress. Sure, there were lots of listings for the parts I needed, but I was struggling to find good prices for the parts. Thankfully, after around 10ish minutes, I was able to find three listings that would allow my project to cost less than 30 dollars! They will all be in the BOM, as well as [on the whiteboard I used](https://miro.com/app/board/uXjVHwO0I8I=/?share_link_id=59015536251). 

Secondly, another tedious task I had to overcome was finding all of the data sheets and wiring data for each component! A major example was the EWAWGIB barcode scanning module. While I was trying to figure out how to wire its TTL interface, I realized it used a ribbon cable (thanks a lot, EVAWGIB 🙄). So, I had to find two things: a converter that would convert the ribbon cable's pins into the standard 2.54mm spacing, and diagram on what pins needed what to run the EVAWGIB safely. Thankfully, I found both of these after around 5ish minutes (look in the images for the diagram and the BOM for the converter)!

### Images
Here's the images for the diagram I made, as well as other images of diagrams and other miscellaneous images:

The full diagram:
<img width="1573" height="904" alt="Screenshot 2026-08-30 at 12 36 24 PM" src="https://github.com/user-attachments/assets/29707a1e-c3b0-40ed-b7ef-6f86570ff3f2" />

The wiring part of the diagram:
<img width="2033" height="907" alt="Screenshot 2026-08-30 at 12 37 11 PM" src="https://github.com/user-attachments/assets/28d9042b-a1bf-4ba8-aebf-641e181bdadf" />

(A very bad) CAD design:
<img width="1208" height="600" alt="Screenshot 2026-08-30 at 12 37 35 PM" src="https://github.com/user-attachments/assets/fd8a274f-a888-46a0-bc05-cdf5cbd433d0" />


The diagram I found (hallelujah!!!):

<img width="750" height="1632" alt="image" src="https://github.com/user-attachments/assets/f8d6fac6-2de4-4877-980d-c097a5797ab0" />

### Links
Here's some of the links to the things I've created so far:

The Design Whiteboard: https://miro.com/app/board/uXjVHwO0I8I=/?share_link_id=880799899556

### Total Hours Spent: 4.5 Hours

## 8/27-8/30
### A Summary Of The Past 3 Days
Wow, those three days went by in a blink! Anyways, these past days, time was poured into the CAD design of the Bathroom Pass, and I'm proud to say the CAD design is finished! I took inspiration from my V1 design and incorporated it into the V2, so there aren't many differences. However, I had to add a mount for the EVAWGIB, and I also had to add a place for the servo, which would move the ID up and down to give it back to the person. 

### Researching 
Firstly, I had to research the dimensions for the main parts I was going to be using in the project, (this did not include the ESP32-C3; I was planning to wire it with a perf board and just hot glue it on), which were the EMAX ES08MD (servo) and the EVAWGIB DP08 (barcode scanner). For the EVAWGIB, I just used the data sheet that I found on 8/25/26 (previous journal entry). It wasn't too hard to find the dimensions for the servo, either; I just went onto GrabCAD and got a .STEP file of the servo and used its dimensions. In the end, I also tested that the parts fit in their mounts (which they thankfully did). 

### Tedious Tasks
Thankfully, I didn't encounter too many harsh problems, so I'm not including them in this journal entry. However, I did have to solve some tedious tasks!

Firstly, one of the major tedious tasks was using the Derived tool in Onshape! The issue I encountered was trying to align the Derived parts using Mate Connectors, which did not align at all! So, once they were placed, I had to manually use the Transform tool to align the parts correctly. However, once they were in position, I could test if the dimensions on the 3D print were correct (which they did). So, in the end, it was worth it :)

### Images
This is for the visual learners out there! :P

The FULL CAD design:
<img width="780" height="895" alt="Screenshot 2026-08-30 at 5 52 55 PM" src="https://github.com/user-attachments/assets/2286e0c3-41bc-4509-bfb1-1221ec004275" />

The CAD design without the parts in their mounts:
<img width="880" height="943" alt="Screenshot 2026-08-30 at 5 53 33 PM" src="https://github.com/user-attachments/assets/1a21aa01-9787-4713-b666-fc7489a39608" />

The Rectangular Pushing Plate (used to align the ID so the servo can push it back up):
<img width="823" height="411" alt="Screenshot 2026-08-30 at 5 54 32 PM" src="https://github.com/user-attachments/assets/a1809b06-475e-43cc-81ad-dfc91b2ed528" />

The EVAWGIB (used for testing the assembly, won't be printed):
<img width="1451" height="989" alt="Screenshot 2026-08-30 at 5 55 33 PM" src="https://github.com/user-attachments/assets/b356b678-4d28-4394-b0be-a96f14185b12" />

### Total Time Spent (Over Past Three Days): 7.5 Hours
