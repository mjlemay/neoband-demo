# neoband-demo
A demo of RFID gate that can be placed on a tablet or laptop with USB RFID reader.

## How to use
This demo assumes a USB RFID reader is connected that will input the RFID as a 10 digit keyboard entry.

It will listen for key presses, check if they are numbers, and go to the next screen if there is a 10 digit number entered.

It will wait ~12 seconds on a load screen by default, and then go to a content screen for 3 minutes before returning to the RFID lock screen.

## To Update

Content can be edited at Line 76.

Variables for time anf ID can be found on Line 91:
```
var LOAD_TIME = 0.20; // minutes
var CONTENT_TIME = 3; // minutes
var ID_LENGTH = 10; // character length
```

CSS colors be set on line 14. They can take six character hexadecimal color values such as `#ff0000` or a red/green/blue/alpha value like `rgba(88, 4, 70, 1)`.