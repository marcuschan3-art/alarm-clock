#define TFT_CS 7
#define TFT_RST 10
#define TFT_DC 8
#define TFT_SCLK 4
#define TFT_MOSI 5

#include <Adafruit_GFX.h>
#include <Adafruit_ST7789.h>
#include <SPI.h>
#include <WiFi.h>
#include "time.h"

const char* ssid = "SpeedBoopsy";
const char* password = "TeslA18@fast";
const char* ntpServer = "pool.ntp.org";

void setup() {
  Serial.begin(115200);
  WiFi.begin(ssid, password);
  const long gmtOffset_set = -28800;
  const int daylightOffset_sec = -28800;
}

void printLocalTime(){
  struct tm timeinfo;
  if(!getLocalTime(&timeinfo)){
    Serial.println("Failed to obtain time");
    return;
  }
}

void loop() {
  Serial.println(&timeinfo, "%H %M %S");
  delay(990);
  
}
