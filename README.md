# servo-controller
4 channel RC servo controller
This project born on necessity to drive some RC classic servo on two programmable positions.
On my model plane i need to drive some servos in two position , like GAS choke servo , fuel pump, other's.....
The controller can drive up to 4 servo, each one can assume two different position, simple pressing a toggle push button. In htis way you can easily move the servo on differetn position li ke for example :
- close the choke, start gas engine and then open choke for normal operation.
- start / stop (dimming )fuel pump
- drive a pwm switch (ingition or others loads)

This circuit can be useful for some function you wan't on your radio or if you don't have enought channel like in my case.

How to use it ? very simple :
- each channel have a push button that toggle the servo position each time is pressed, a led show the status. (min/ max position)
- a second main function is the programmation phase, each channel can be programmed with 3 buttons , so you can adjust minimum / maximum duty (position) for each channel.

Power supply is 5V, but can operate also at 6 or 7.2V if you like. (be careful when you power on the board, no protection are provided for reverse polarity.)
Microcontroller used it's a bit old, NXP MC9S08GT32CFBE from NXP (previous Freescale) but still in full production, i have used this one because i have them from old projects, it's much more powerful that required, but easy to use. To program the uP you need BDM interface, from P&E or from openBDM, serch them with google, tools are free from NXP web site. 

A green led blink slow means the processor is running.

How to :
by default each servo position have two values, 1000uS pulse as minimum and 2000uS pulse as maximum, press a button (SW1 to SW4) toggle the corresponding servo position and red LED near each push button.

You have other 3 push button, SW5 (UP) SW6 (down) SW7 (ENTER), to enter in programming mode press for 3" the SW7.
When in programming mode all red leds will blink quickly, now press one pushbutton from SW1 to SW4 to select the channel servo you want calibrate / programming, corresponding led will be off or on (depend how many time you press the button), each time corresponding led toggle and servo follow the programmed values, press SW5 UP or SW6 DOWN to adjust the servo position you like, make it for MIN position (led off) and MAX position (led on), repeat it as you like until the two servo positions are right for your requirements.

Now press again SW7 (ENTER) for 3" to save the values. 

Remember : at power on the servo will take position saved with led off, keep in mind when you make the calibration.

