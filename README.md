# alarm-clock
Alarm clock for BLARE

Important!!!: Download the finalalarmclockv2.step, then view it in a step file viewer!
Note: This is my second time, I restarted becuase there was tons of problems in my first design.

BILL OF MATERIALS: 1x Lolin C3 Mini ESP 32 Devboard, 6 Keyboard Switches, 1 2.25in TFT Screen, 1 3.3V Piezo Buzzer, 10 M-M Jumper Cables, 10 F-M Jumper Cables, 10 F-F Jumper Cables

I created a alarm clock that displays the time by connecting to wifi and getting the time from pool.ntp.org. I built becauase I want experience in designing(CAD), soldering/wiring, and Aurduino coding. Some challanges I faced were being a complete beginner to CAD and Aurduino coding.(I will also need to learn how to solder)


- Planning: I want square alarm clock but with rounded edges. I want it to find the current time and display it.                                                                      


- Planned wiring (The wires are straight becuase I suck at drawing)

<img width="954" height="696" alt="Screenshot 2026-07-09 at 4 00 27 PM" src="https://github.com/user-attachments/assets/e7870747-5ae9-46db-a16c-884688dd0361" />


- Made the fastened mate, created the case, and extruded the case.
Learned how to attach objects, and extrude.

<img width="562" height="309" alt="Screenshot 2026-07-09 at 9 20 22 AM" src="https://github.com/user-attachments/assets/eabebf3e-a5ab-494b-add4-427550a45d1a" />



- Added keyboard switch extrusions.
Learned how to upload DXF file and do a intrusion.
<img width="410" height="217" alt="Screenshot 2026-07-09 at 9 45 45 AM" src="https://github.com/user-attachments/assets/02ae6728-e096-453c-8096-b1f84f309f07" />

- Added buzzer hole

<img width="189" height="199" alt="Screenshot 2026-07-09 at 9 51 11 AM" src="https://github.com/user-attachments/assets/85e0f8f2-c826-4aff-87e1-d9bed12f7d81" />

- Added extrusions

<img width="65" height="43" alt="Screenshot 2026-07-09 at 3 07 48 PM" src="https://github.com/user-attachments/assets/16c9100d-6cc5-4f51-b0bd-8c0f33ecaf2e" />

- Added keyboard switches
<img width="812" height="647" alt="Screenshot 2026-07-09 at 3 06 39 PM" src="https://github.com/user-attachments/assets/89dae250-f691-4986-ac93-3e63e3fb6442" />

I forgot to screenshot but here's what I did for coding

1 Included WiFi.h, time.h, and SPI.h   
2 Added ssid and password so the Esp could connect to wifi     
3 Added a const char for pool.ntp.org called ntpServer    
4 Made a function called printLocalTime which got the time from ntpServer and printed the hour, minute, and second   every 990 milliseconds
5 Added a function for a buzzer   
