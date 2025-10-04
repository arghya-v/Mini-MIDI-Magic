Blueprint bot overwrote my journal, so here it is again

---
Title: "My custom MIDI controller"
Author: "Arghya Vyas"
Description: "A simple MIDI controller I made!"
Created On: "29/9/2025"
---

Note: I kinda forgot I had to journal, but luckily I have screenshots of questions I asked during Slack, so I will use those from the 24th - 29th of September

# September 24th (8PM-10PM)

I started by looking at the mini MIDI magic guide. Alognside that I also installed KiCad and started to learn how it works. I also learned about the switch matrix system, and decided to implement that in my project. 
Initially, I was confused about the switch matrix and what it meant, but I figured it out and got started by making 4 rows like this

<img width="843" height="354" alt="image" src="https://github.com/user-attachments/assets/9a16a227-3e87-4bd9-b349-d0800656fc15" />
<br></br>

# September 26th (7PM - 9PM)

After I made my rows, I started to work and learn about rotary encoders, initially, I had made a 6x6 matrix, but I realized that I only need a 4x5 matrix, and I leave the other 2 rows for my rotary encoders.
It took me a while to figure it out, because I was new to making schematics, but I luckily got some help on the slack, and then made a schematic like so:
<img width="666" height="712" alt="image" src="https://github.com/user-attachments/assets/edfdcaf9-0c04-42ce-8a3b-9421a3c43898" />
<img width="743" height="413" alt="image" src="https://github.com/user-attachments/assets/3e468e5d-c858-4774-96f3-dbbc6cf6a1c9" />
<br></br>

# September 27th (10AM - 12 Noon)

I then proceeded to add on the SD card and LCD screen, I decided to stick with the guide here, because I am new. The LCD was pretty easy to add, but I had to ask some questions regarding the SD card because there wasn't a full screenshot for it. In the end I got it working though.

<img width="449" height="363" alt="image" src="https://github.com/user-attachments/assets/aa49eb69-5784-4314-9f32-883adc959143" />
<br></br>

# September 29th (8AM - 9AM)
To finish off, I got my work checked over, fixed an issue with the switches, and then did some organizing. 
This was my final BASE schematic. 
<img width="1133" height="818" alt="image" src="https://github.com/user-attachments/assets/2c0057c4-3787-401c-95b4-5880e9a3abba" />
<br></br>
I am hoping to add a slide, potentiometer later on and customize it to my liking.
# September 29th (5PM - 7PM)

After some reasearch, I figured out that I needed more ADC pins, so I looked into another breakout board and came across the ADS1015, I then implemented it, and found a footprint online that I could use.
After that, I made a simple linear slide potentiometer footprint, and found a 7.5mm one on Adafruit, I then connected it to the ADS breakout board. 

<img width="754" height="875" alt="image" src="https://github.com/user-attachments/assets/9a88d5a9-9901-46d5-b0f3-113b3084c4d0" />

# September 30th (5PM - 6PM)

I made the footprint of the I2S DAC module, I efficiently used the .brd file, imported it into kicad, then copied the footprint over. 

<img width="734" height="475" alt="image" src="https://github.com/user-attachments/assets/4adc928a-a1ee-458f-a26c-1400ed8d4895" />
<br></br>

# October 1st (5PM - 6:30)

I had to refine my schematics and footprints for my I2S DAC, so I updated them and cross checked the correct pins

<img width="657" height="664" alt="image" src="https://github.com/user-attachments/assets/1d6ca7ce-cff3-428a-b2bb-4b771b159e23" />
<br></br>

# 6:30PM - 8:20 PM
I finally converted to a PCB and arranged my parts
<img width="1069" height="553" alt="image" src="https://github.com/user-attachments/assets/e797a425-755e-4c07-a439-444a6843b6e1" />

# October 2nd, 5PM-7PM

I routed my PCB, I kept it simple with an autorouter.
<img width="1117" height="638" alt="image" src="https://github.com/user-attachments/assets/415b5e0e-f8db-4928-b1c6-6fec6b3473cc" />
<br></br>
I also decided to work on my chassis after, to keep it simple, I just used TinkerCad. I added my PCB as a .stl file and started working on the base
<img width="1028" height="791" alt="image" src="https://github.com/user-attachments/assets/fa09b2f9-0256-4f5e-8bd8-2820617a4b26" />
<br></br>

# October 3rd, 5PM-7:50PM

I continued to work on some CAD for the chassis, I added internal supports, some keyswitches for refererence, and some barriers on the side.
<img width="1359" height="914" alt="image" src="https://github.com/user-attachments/assets/ba07f51c-4c33-47be-8c56-51746dc6d8fa" />
<br></br>

<img width="610" height="607" alt="image" src="https://github.com/user-attachments/assets/4f479bba-e3f0-4df3-8f52-244de3f9ab1d" />
<br></br>

# October 4th, 12 noon - 2PM

I worked on the top plate, kept it at a height of 1.5mm since thats the standard for keyboards, also made holes for the jumpers and encoders

<img width="1350" height="864" alt="image" src="https://github.com/user-attachments/assets/5b605f69-3bd0-4d84-8007-1261eebe4b0f" />
<br></br>
