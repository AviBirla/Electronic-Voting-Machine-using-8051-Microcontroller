# Electronic-Voting-Machine-using-8051-Microcontroller

Electronic voting machine has now replaced the traditional mechanism of voting due to several advantages like security, automatic counting etc. This project presents a way to develop an electronic voting machine which displays the count of votes on a 16x2 LCD interface. A user can get his/her vote register through a set of switches (one for each candidate). After every cast of vote, the subsequent count can be seen on LCD. The circuit uses AT89C51 microcontroller and the code for the project has been written in C.

This LCD based electronic voting machine is designed for four candidates. The input part consists of a set of six tactile switches. The switches and 16×2 LCD are interfaced to microcontroller AT89C51 for various operations and displays.
 
The provision of casting votes for the candidates has been provided through four of these switches. These switches are made active high and connected to pins 2-5 (P1^1 – P1^4) of the controller. The remaining two switches (both active low) are to start and stop the voting procedure. They are connected to pins 1 and 6 (P1^0 and P1^5) respectively. The Init (start) switch initializes the voting system when pressed, while the Stop switch ends the voting and displays the poll results on LCD screen.
 
For more details on working with LCD, refer LCD interfacing with 8051. The data pins of the LCD (pins 7-14) are connected to the output port P2 of the microcontroller. The control pins (RS, R/W and EN) are connected to port P3 pins P3^0, P3^1 & P3^6 respectively.

Working : 

The voting is started by pressing the Init switch after which the user is prompted to vote. The count of votes is stored in four different variables. As soon as the user votes for a candidate by pressing one of the switches, the value of the corresponding variable is increased by one. After this a Thank you message is displayed on LCD to acknowledge the registration of user’s vote.
The message stays on the screen until the next user either presses the Init button to cast another vote or Stop switch is pressed get the poll results. When the stop button is pressed, the names of the candidates are displayed along with their vote counts. After some delay, the result is displayed which could be either declaration of the winner candidate or the candidates with a clash of their number of votes.

► Components :

♦ AT89C51 Microcontroller

♦ I2C LCD

♦ Resistors , Capacitors , Jumper wires , 6 Switches , a medium size breadboard.

♦ Crystal Oscillator
