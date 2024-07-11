[![Build_special_firmware](https://www.nn-digital.com/wp-content/uploads/2019/07/NodeMCU-Lolin-1.jpg)](https://github.com/dannywilliam/DW-JWS-ESP_Rev-1/blob/main/README.md)
# DW JWS ESP_Rev 1
Jadwal Waktu Sholat yang dibuat dengan ESP8266 dan Panel P10 (HUB12)


## Catatan : 
 * Perlu Power Eksternal 5V ke LED P10.
 * Sumber awal source code : https://github.com/busel7/Arduino/tree/master/MembuatJWS
 * Pin Buzzer memakai GPIO 2 (D4), disesuaikan dengan skematik Khalifah JWS.
 * Jumlah Panel 1 x 1.
 * Fitur lain akan disesuaikan dengan kebutuhan.

## Fitur
 * Jam Besar.
 * Jadwal Waktu Solat dan Tanbih Imsak
 * Alarm Adzan Solat dan Tanbih Imsak
 * Tanggal Masehi
 * Tanggal Hijriyah
 * Hitung Mundur Iqomah
 * Running Text Nama Masjid

## Wifi
 * SSID = DW JWS ESP
 * PassWord = 123456789
 * IP Address : 192.168.4.1

## Komponen yang dibutuhkan
 * Microcontroller berbasis ESP8266 (NodeMCU, Wemos D1 Mini, atau yang sejenisnya).
 * RTC DS3231.
 * Panel P10 (HUB12).
 * Buzzer.
 * Adaptor/Power Supply 5v.
 * Kabel.

## Pin on DMD LED P10 Panel

| DMD P10 | GPIO | NODEMCU | 
| ------- | ---- | ------- |
| A       | GPIO16 | D0    |                                                 
| B       | GPIO12 | D6    |                                                  
| CLK     | GPIO14 | D5    |                           
| SCK     | GPIO0  | D3    |                           
| R       | GPIO13 | D7    |
| NOE     | GPIO15 | D8    |
| GND     | GND    | GND   |

## Pin on RTC DS3231

| DS3231 | NODEMCU |
| ------ | ------- |
| SCL    | D1 (GPIO 5) |
| SDA    | D2 (GPIO 4) |
| VCC    | 3V          |
| GND    | GND         |

## Pin on Buzzer

| Buzzer | NODEMCU |
| ------ | ------- |
| +      | D4 (GPIO 2) |
| -      | GND         |

## Eksternal Library
 * DMDESP : https://github.com/busel7/DMDESP
 * PrayerTime : https://github.com/asmaklad/Arduino-Prayer-Times
 * RTC DS3231 : https://github.com/Makuna/Rtc
 * ArduinoJson V6 : https://github.com/bblanchon/ArduinoJson
 * F1kM_Hisab : https://github.com/wardi1971/F1kM_Hisab

## Tools : 
 * Desain bitmap dan font : http://dotmatrixtool.com
 * LittleFS Uploader : https://github.com/earlephilhower/arduino-esp8266littlefs-plugin/releases
