# The ID Eater
A bathroom pass that has the ability to scan a school ID's barcode and output the ID onto a Hall Pass monitor. 

Hey fellow viewer! I'm Ayaan, a 13 year-old who's spent ~1.5 working with [Hack Club](hackclub.com)! I made this project tailored for my school (however feel free to use it under the MIT license)!

Below you'll find out what this project is, how it works, and the BOM (Bill Of Materials) and CAD to build it yourself!

## What it is
What the heck is this project, anyway? 

Well, to summarize it, it's a device that automatically scans a student's school ID (find what it looks like in the images section) and gives the student a virtual hall pass (using the software [5starstudents](5starstudents.com)). Then, when the student wants to check back in, they simply click a button, which gives the student their ID back and takes away their hall pass. Simple!

## How it works
How does this project work, anyway? Well, it has several components that give the project its abilities: the EVAWGIB DP08 Barcode Scanner, the EMAX ES08MD Servo, the ESP32-C3, a perf board, and a FFC/FPC Converter. Below, you'll see how each component is used:

### EVAWGIB DP08 1D Barcode Scanner
This component scans the barcode on the ID, and hands over the ID number to the ESP32-C3 for further processing. That's it!

### EMAX ES08MD Servo
This component moves the ID up and down, so when the student is gone, the ID will move down, and vice versa. Pretty simple, huh?

### ESP32-C3 
This component is the brains of the Bathroom Pass, making it the most important piece; without it, nothing would function! When the EVAWGIB scans the ID, it is given to the ESP32, which takes that and connects to a Chromebook to sign the person out. At the same time, the ESP32 also moves the servo to move the ID down while the student has gone to the bathroom.

### Perf Board
If you don't know what a Perf Board is, think of it like a solderable breadboard! However, instead of the connections being removable, they are permanently soldered on, which is perfect for prototypes and actual projects! In this case, the Perf Board is used to wire everything together.

### FFC/FPC Converter
If you don't remotely know what this is, I don't blame you! I didn't know until recently... 😅

Anyways, this is a device that converts a ribbon cable output to the standard 2.54mm spaced pin layout. Annoyingly, the EVAWGIB uses a ribbon cable, so if you to wire the EVAWGIB to the ESP32-C3, you'd need to use this converter. 

## BOM (Bill Of Materials)
Here's the Bill Of Materials if you want to build this yourself:

| Item | Price | Link |
| -----|-------|-----|
| EVAWGIB 1D Barcode Scanner | $13.90 | [Link](https://t.ly/4ARFP) |
| EMAX ES08MD Servo | $5.59 | [Link](https://t.ly/3Bg_y) |
| ESP32-C3 | $2.59 | [Link](https://t.ly/GQSVB) |
| Perf Board | $1.99 | [Link](https://t.ly/8iwan) |
| FFC/FPC Converter | $1.99 | [Link](https://t.ly/gyBrI) |

### Total (+ tax and shipping): $36.68

## Images
Visual learners rejoice!!!!!!

### The Design ([Here's the link if you want it](https://miro.com/app/board/uXjVHwO0I8I=/?share_link_id=500169589295)):
<img width="1563" height="883" alt="Screenshot 2026-08-30 at 6 41 34 PM" src="https://github.com/user-attachments/assets/1d62b553-9b00-4002-9bd0-19964badc67c" />

### The CAD:
<img width="1001" height="937" alt="Screenshot 2026-08-30 at 6 42 24 PM" src="https://github.com/user-attachments/assets/97018643-bed7-42ad-8858-67cf985a438e" />

