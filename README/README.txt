IMPROVING THE LIVES OF VISUALLY IMPAIRED INDIVIDUAL WITH IOT POWERED COMPANION TECHNOLOGY
-----------------------------------------------------------------------------------------

FUNCTIONALITYS:
--------------
1) OBSTRACLE DETECTION
2) WATER DETECTION
3) SOS COMMUNICATION
4) LIVE LOCATION TRACKING
5) STICK IDENTIFICATION

SYSTEM REQUIREMENTS:
-------------------

HARDWARE REQUIREMENTS:
---------------------
1) ESP WROOM 32
2) ULTRASONIC SENSOR
3) MOISTER SENSOR
4) GPS
5) BUZZER
6) JUMPER WIRE
7) BATTERY
8) PUSH BUTTON
9) ESP WROOM 32 EXTENSION BOARD

SOFTWARE REQUIREMENTS:
---------------------
1) ARDUINO IDE
2) BLYNK APPLICATION

STEP BY STEP INSTRUCTIONS:
--------------------------

[NOTE : LANGUAGE USED -> EMBEDDED C]

STEP 1 : INSTALL THE ARDUINO IDE FROM THE BROWSER.

STEP 2 : DOWNLOAD THE ESP WROOM 32 BOARD [TOOLS->BOARD->MANAGE->ESP WROOM 32/ ESP DEV BOARD].

STEP 3 : DOWNLOAD THE CP210X DRIVER FROM THE BROWSER [ONLY IF YOU ARE USING THE ESP 32 CONNECTION FOR THE FIRST TIME WITH YOUR LAPTOP].

STEP 4 : CHOOSE THE PORT NUMBER(COM PORT) [TOOLS->PORT->COM 6(CONNECT THE ESP WROOM 32 WITH THE LAPTOP USING A USB TO SEE THE COM 6 PORT)].

STEP 5 : DOWNLOAD THE REQUIRED LIBRARYS AS GIVEN BELOW [SKETCH->INCLUDE LIBRARY->MANAGE LIBRARY->TYPE THE REQUIRED LIBRARY NAME AND
         CLICK ON INSTALL, IF NOT AVAILABLE TAHN DOWNLOAD THE SPECIFIC LIBRARY FROM THE GITHUB AND ADD THE ZIP FOLDER(SKETCH->
         INCLUDE LIBRARY->ADD ZIP->COOSE THE LIBRARY ZIP FOLDER FROM THE DOWNLOADS)].
   
                                1) WiFiClient.h

                                2) BlynkSimpleEsp32.h

                                3) WiFiClientSecure.h

                                4) TinyGPS++.h

                                5) UniversalTelegramBot.h

STEP 6 : USE "->" TO UPLOAD THE CODE INTO THE ESP WROOM 32.

STEP 7 : TO CHANGE THE EXISTRING CODE CHANGE THE FOLLOWING:
                                                                                                      --
             SSID                              : (YOUR HOTSPORT NAME)                                  |
                                                                                                       |---> COPY FROM YOUR PHONE HOTSPORT 
             PASS                              : (YOUR HOTSPORT PASSWORD)                              |
                                                                                                      --
                                                                                                      --
             TEMPLATE NAME                     : (CHANGE YOUR BLYNK APP TEMPLATE NAME)                 |
                                                                                                       |
             TEMPLATE ID                       : (CHANGE YOUR BLYNK APP TEMPLATE ID)                   |--->COPY FROM BLYNK APP TEMPLATE
                                                                                                       |
             AUTHENDICATION TOKEN              : (CHANGE THE TEMPLATE AUTHENDICATION TOKEN)            |
                                                                                                      --
                                                                                                      --
             TELEGRAM BOT ID                   : (CHANGE THE TELEGRAM BOT ID)                          |
                                                                                                       |---> GET FROM TEKEGRAM BOT
             TELEGRAM BOT AUTHENDICATION TOKEN : (CHANGE TEH TELEGTRAM BOT AUTHENDICATION TOKEN)       |
                                                                                                      --

STEP 8 : INSTALL TELEGRAM AND LOGIN INTO THE APPLICATION.

STEP 9 : CREATE THE TELEGRAM BOT.

STEP 10 : INSTALL BLYNK APPLICATION AND LOGIN INTO THE APPLICATION.

STEP 11 : CREATE NEW TEMPALTE AND GIVE THE NAME.
 
STEP 12 : CLICK ON "+" SYMBOL TO ADD THE FOLLOWING WIDGETS TO THE BLYNK DASHBOARD: 
                    
                            1) VALUE DISPLAY --> NAME IT AS [LATITUDE]      --> CREATE A DATA STREAM AND SELECT A VARAIABLE V0
                            2) VALUE DISPLAY --> NAME IT AS [LONGITUDE]     --> CREATE A DATA STREAM AND SELECT A VARAIABLE V1
                            3) VALUE DISPLAY --> NAME IT AS [LOCATION LINK] --> CREATE A DATA STREAM AND SELECT A VARAIABLE V2
                            4) GAUGE         --> NAME IT AS [SPEED]         --> CREATE A DATA STREAM AND SELECT A VARAIABLE V3
                            5) ON/OFF BUTTON --> NAME IT AS [FOUND STICK]   --> CREATE A DATA STREAM AND SELECT A VARAIABLE V4

STEP 13 : CHANGE THE COLOR AND ALIGNMENT AND CUSTOMIZE AS YPUR WISH.

STEP 14 : CLICK ON SAVE BUTTON. 

CIRCUIT CONNECTION:
-------------------

[ NOTE : CONNECT ALL THE PIN ON THE ESP WROOM 32 EXTENSIOIN BOARD 
USING FEMALE TO FEMALE JUMPER WIRE AND CONNECT THE ESP WROOM 32 
WITH ITS EXTENSION BOARD AND CONNECT THE COMPONENTS AS GIVEN BELOW]
   
1) ULTRASONIC SENSOR CONNECTION:

          TRIG PIN = 13
          ECHO PIN = 12
          GND PIN  = GND(12/13)
          VCC PIN  = VCC(12/13)

2) MOISTER SENSOR CONNECTION:

          A0 PIN   = 18
          GND PIN  = GND(18)
          VCC PIN  = VCC(18)

3) GPS CONNECTION:

          TX PIN   = 17           
          RX PIN   = 16
          GND PIN  = GND(16/17)
          VCC PIN  = VCC(16/17)

4) BUZZER CONNECTION:

          POSITIVE PIN(+VE) = 5
          NEGATIVE PIN(-VE) = GND(5)

5) PUSH BUTTON CONNECTION:

          POSITIVE PIN(+VE) = 2
          NEGATIVE PIN(-VE) = GND(2)

[IMPORTANT INSTRUCTIONS] - " DO NOT DO THESE " 
-----------------------------------------------

1] DO NOT PLACE ANY COMPONENT ON THE METAL SURFACE WHILE EXECUTION TO AVOID SHORT CIRCUIT.

2] CONNECT THE PIN  PROPERLY AS PER THE PIN CONNECTION WHICH IS GIVEN ABOVE , IF NOT THE COMPONENT MAY GET SHORT.

3] KEEP THE COMPONENTS AWAY FROM WATER TO AVOID SHORT CIRCUIT.

4] DO NOT DUMP/INSERT THE CODE INTO THE ESP WROOM 32 WHILE IT IS CONNECTED WITH THE SENSORS
 - REMOVE IT FROM THE EXTENSION BOARD EVERY TIMEN BEFORE DUMP/INSERTING THE CODE.

5] PRESS THE BOOT BUTTON ONCE WHEN THE CODE GET START UPLOADING. 

6] DO NOT REMOVE THE CONNECTION WHILE UPLOADING THE CODE SO THE BOARD MAY GET CORREPT.

7] DO NOT GIVE MORE POWER SUPPLY MORE THAN 3.3V WITHOUT ANY PROTECTION.

8] HANDLE ALL THE COMPONENTS WITH CARE.
