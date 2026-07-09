# alarm-clock
Alarm clock for BLARE

Important!!!: Download the finalalarmclockv2.step, then view it in a step file viewer!
Note: This is my second time, I restarted becuase there was tons of problems in my first design.

BILL OF MATERIALS: 1x Lolin C3 Mini ESP 32 Devboard, 6 Keyboard Switches, 1 2.25in TFT Screen, 1 3.3V Piezo Buzzer, 10 M-M Jumper Cables, 10 F-M Jumper Cables, 10 F-F Jumper Cables



Planning: I want square alarm clock but with rounded edges. I want it to find the current time and display it.                                                                      


Planned wiring (The wires are straight becuase the wires would've crossed due to my horrible drawing skills)

<img width="954" height="696" alt="Screenshot 2026-07-09 at 4 00 27 PM" src="https://github.com/user-attachments/assets/e7870747-5ae9-46db-a16c-884688dd0361" />


Made the fastened mate, created the case, and extruded the case.
Learned how to attach objects, and extrude.

<img width="562" height="309" alt="Screenshot 2026-07-09 at 9 20 22 AM" src="https://github.com/user-attachments/assets/eabebf3e-a5ab-494b-add4-427550a45d1a" />



Added keyboard switch extrusions.
Learned how to upload DXF file and do a intrusion.
<img width="410" height="217" alt="Screenshot 2026-07-09 at 9 45 45 AM" src="https://github.com/user-attachments/assets/02ae6728-e096-453c-8096-b1f84f309f07" />

Added buzzer hole

<img width="189" height="199" alt="Screenshot 2026-07-09 at 9 51 11 AM" src="https://github.com/user-attachments/assets/85e0f8f2-c826-4aff-87e1-d9bed12f7d81" />

Added extrusions

<img width="65" height="43" alt="Screenshot 2026-07-09 at 3 07 48 PM" src="https://github.com/user-attachments/assets/16c9100d-6cc5-4f51-b0bd-8c0f33ecaf2e" />

Added keyboard switches
<img width="812" height="647" alt="Screenshot 2026-07-09 at 3 06 39 PM" src="https://github.com/user-attachments/assets/89dae250-f691-4986-ac93-3e63e3fb6442" />


Code:
#define TFT_CS 1
#define TFT_RST 2
#define TFT_DC 3
#define TFT_SCLK 4
#define TFT_MOSI 5

#include <Adafruit_GFX.h>
#include <Adafruit_ST7789.h>
#include <SPI.h>
#include <WiFi.h>
#include "time.h"

const char* ssid = SpeedBoopsy;
const char* password = TeslA18@fast;
const char* ntpServer = "pool.ntp.org";

void setup() {
  Serial.begin(115200);
  WiFi.begin(ssid, password);
  
}

void loop() {
  serial.println(ntpServer)
  delay(10000)
}

