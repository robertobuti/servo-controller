# servo-controller
4 channel RC servo controller
This project born on necessity to drive some RC classic servo on two programmable positions.
On my model plane i need to drive some servo in two position , like GAS choke servo , fuel pump, other's.....
The controller can drive up to 4 servo, each one can assume two different position, simple pressing a toggle push button. In htis way you can easily move the servo on differetn position li ke for example :
- close the choke, start gas engine and then open choke for normal operation.
- start / stop (dimming )fuel pump
- drive a pwm switch (ingition or others loads)

This circuit can be useful for some function you wan't on your radio or if you don't have enought channel like in my case.

How to use it ? very simple :
- each channel have a push button that toggle the servo position each time is pressed, a led show the status. (min/ max position)
- a second main function is the programmation phase, each channel can be programmed with 3 buttons , so you can adjust minimum / maximum duty (position) for each channel.

Power supply is 5V, but can operate also at 6 or 7.2V if you like.
Microncontroller used it's a bit old, NXP MC9S08GT16CFB from NXP (previous Freescale) but still in full production, i have used this one because i have them from old projects, it's much more powerful that required, but easy to use. To program the uP you need BDM interface, from P&E or from openBDM, serch them with google, tools are free from NXP web site. (CodeWarrior 10.6 has been used)


