YSZ-4 Four Digit Electronic Clock Instruction Manual  
“C51 4 bit Clock Kit” 

YSZ-4 four electronic clock, it uses an AT89C2051 as its core, a total of 16 electronic components to create a clock with hours/minutes or minutes/seconds, two independent alarms, (8:00 -20:00) hourly chime, accurate adjustment, and other functions. 
1> Rationale 
The whole system by MCU minimum system, key input circuit, display circuit, buzzer circuit and power supply parts. 
1. MCU minimum system includes the U1 (AT89C2051), C1, R1 for power on reset circuit .Clock circuit is composed of C2, C3 and Y1. 
2. The pressed key input circuit is composed of S1, S2, short press the button once a loud buzzer rang, long press the button once two loud buzzer rang. 
3. The display circuit： 4 bits common cathode and one PR1 resistors pack. 
4. Buzzer circuit is composed of Q1, R2 and LS1, short press the button once a loud buzzer rang, long press the button once two loud buzzer rang. 
5. J1 is 5v power supply input terminal, C4 filtering. 
2>Operation instructions 
It will display 12:59 when Power-on, while is normal interface ("hours:minutes"). The both channels of the alarm clock are opened. At the same time, the first alarm clock has been set at 13:01.the second alarm clock has been set at 13:02. 
After power on, short press S2.The display of digital tube will switch between "hours:minutes" and "minutes:seconds". 
Long press S1 to enter the system Settings menu. There are A, 8, C, 0, E, F, G, H, I submenus. 
Short press S1 to cycle through the submenus, and finally back to the normal display. 
A Sub menu: Correction for hours 
A 
Display data will add 1 with each press of S2. When done adjusting the A Submenu, short press S1 to save the setting, quit the A submenu, and enter the B submenu. 
B Sub menu: Correction for minutes 
8  
Display data will add 1 with each press of S2.  When done adjusting the B Submenu, short press S1 to save the setting, quit the B submenu, and enter the C submenu. 
C SCub  menu: on time alarm switch 
The default state is ON (on-time-alarm is open from 8:00 to 20:00) 
It will switch between ON and OFF (hourly alarm is disabled) with each press of S2. Short press S1 to save the setting, quit the C submenu, and enter the D submenu. 
D Submenu: The first alarm-clock switch 
0 
The default state is ON (the first alarm-clock is opened) 
It will switch between ON and OFF (first-alarm-clock is closed) when press S2。 If set to ON, short press S1 to save and quit, then enter E submenu; 
If set to OFF, short press S1 to save and quit, then enter G submenu; 
E SEub  menu: The first alarm clock set for hours 
Display data will add 1 with each press of S2. When done adjusting the E submenu, a short press of S1 will save the setting, quit the E submenu, and enter the F submenu. 
F Sub menu: The first alarm clock set for minutes 
F 
Display data will add 1 with each press of S2.  When done adjusting the F Submenu, a short press of S1 will save the setting, quit the F submenu, and enter the G submenu. 
G Submenu: The Second alarm-clock switch 
G 
The default state is ON (the second alarm-clock is enableded) 
It will switch between ON and OFF (second-alarm-clock is closed) when S2 is pressed. If set to ON, short press S1 to save/quit, and enter H submenu; 
If set to OFF, short press S1 to save/quit, and enter normal interface; 
H Sub menu: The second alarm clock set for hours 
H 
Display data will add 1 after each press of S2. When done setting the F Submenu, a short press of S1 will save the setting, quit the H submenu, and enter the I submenu. 
I SuI b menu: The second alarm clock set for hours 
Display data will add 1 after each press of S2. When done setting the I Submenu, a short press of S1 will save the setting, quit the H submenu, and enter the normal interface. 
Seconds correction: 
Short press S2 in the normal interface, to enter "minutes:seconds" interface. Long press S2 will make the second zero and stop the clock. Then a short press of S2 twice will start the clock and enter the normal interface. 
3>Schematic circuit diagram 
Note: there is direction for PR1 Resisters Packs, there is one pad on the board that has a square drawn around it on the silkscreen which is pin 1. The resistor pack has a dot near one pin that indicates it is pin 1.   

4>Component list 
 
                       NEME                    Type/Spec               Identifier     Specific
                                                                                       orientation?
                                                                                       
               01      Resistor                10K                     R1             No 
               02      Resistor                10K                     R2             No 
               03      Ceramic Cap             30pf                    C2             No 
               04      Ceramic Cap             30pf                    C3             No 
               05      Ceramic Cap             104pf                   C4             No 
               06      Electrolytic Cap        10uF / 25v              C1             YES 
               07      Resistor Pack           1K                      PR1            YES 
               08      Crystal                 12MHz                   Y1             No 
               09      Transistor              8550                    Q1             YES 
               10      Tact Switch             6*6*5                   S1             YES 
               11      Tact Switch             6*6*5                   S2             YES 
               12      IC Socket               20pin                   U1             YES 
               13      MCU                     AT89C2051               U1             YES 
               14      Buzzer                  5v active               LSI            YES 
               15      Digital Display         4 position 7- segement  DS1            YES 
                                                module
                                                
               16      DC connector            2 position 3.5mm        J1             YES 
                                                terminal block
                                                
               17      PCB                     52*42mm 

