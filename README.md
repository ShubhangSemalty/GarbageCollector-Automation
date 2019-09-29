# GarbageCollector-Automation

This project was created to demonstrate surveillance type approach to the current garbage bin collection system where verification is done using RFID tags. The idea is that each garbage truck when collecting the garbage from a common big dump needs to swipe the card at the Card Reader that is to be placed on the garbage dump. In case the card is a 100% match with the prestored credentials, then a signal will be sent from the garbage dump using a radio sensor (nRF in this case, it can be replaced with a narrowband radio sensor or also a LORA sensor). THe leads to a server that is within a well defined range (100m for nRF and 1Km for LORA). The common server then using internet logs the data directly to a google sheet using a small Google Script which I would upload in a little while. If there is no card swiped within a period of 24 hours, then we register a complaint.

DEPENDANCIES

Radio connection is established wihtout any issue.
RFID is correctly read.
Radio transmission takes place properly.
Equipment used:

Arduino UNo
Breadboard
nRF sensors (1 for transmission and one for receival.
RFID Card reader by REES52 ( only a single unit)
Capacitors: 100uF / 25V for nRF sensors (Spherical type)
Jumper wires.
Buzzer
ESP8266 (for server side programming and data transfer)
