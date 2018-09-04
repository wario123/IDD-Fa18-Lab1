# IDD-Fa18-Lab1: Blink!

**A lab report by John Q. Student**


> Include your responses to the bold questions on your own fork of the lab activities. Include snippets of code that explain what you did. Deliverables are due next Tuesday. Post your lab reports as `README.md` pages on your GitHub, and post a link to that on your main class hub page.

We've copied the questions from the lab here. Answer them below!

## Part A. Set Up a Breadboard

[insert a photo of your breadboard setup here]


## Part B. Manually Blink a LED

**a. What color stripes are on a 100 Ohm resistor?**

Brown, Black, Brown
 
**b. What do you have to do to light your LED?**

I have to push the button to light the LED. The Metro Mini also needs to be connected to a power source.

## Part C. Blink a LED using Arduino

### 1. Blink the on-board LED

**a. What line(s) of code do you need to change to make the LED blink (like, at all)?**

When uploading the code to the Arduino, the LED blinks on and off every second. pinMode and digitalWrite functions need to take in as argument either LED_BUILTIN or 13.

**b. What line(s) of code do you need to change to change the rate of blinking?**

We need to adjust the argument of at least one of the delay functions. Increasing or decreasing the first delay function will respectively increase or decrease the time that the LED is lit while increasing or decreasing the second delay function argument will respectively increase or decrease the time that the LED is not lit.

**c. What circuit element would you want to add to protect the board and external LED?**

You would want to add a resistor to limit current going through.
 
**d. At what delay can you no longer *perceive* the LED blinking? How can you prove to yourself that it is, in fact, still blinking?**

Once both delay function arguments are set at 15 ms, I can no longer perceive the LED blinking. To prove that it is, I can take a "Slo-Mo" video with iPhone and by going frame by frame I can notice the LED being off almost half of the frames.

**e. Modify the code to make your LED blink your way. Save your new blink code to your lab 1 repository, with a link on the README.md.**

[Modified Code!](https://github.com/wario123/IDD-Fa18-Lab1/blob/master/partC_question1e.ino)
    

### 2. Blink your LED

**Make a video of your LED blinking, and add it to your lab submission.**

[link to your video here; feel free to upload to youtube and just paste in a link here]


## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**

The LED is able to glow the whole turning range of the potentiometer. Depending on the direction you turn the knob, the LED brightens up or dims down.


## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**

The first thing to do is to change the "int led = 9" to "int led = 11". In order to control how fast it fades, we can change the fadeAmount variable.

**b. What is analogWrite()? How is that different than digitalWrite()?**

analogWrite() is able to generate a wave of specified duty cycle and therefore set the voltage to HIGH/LOW a certain fraction of the time. This fraction changes linearly with how one changes the value for the analogWrite function. It is different than digitalWrite in that digitalWrite can also only have 2 settings: HIGH or LOW but always 100% of the time. analogWrite(255) = digitalWrite(HIGH) and analogWrite(0) = digitalWrite(LOW).


## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**

**d. Is information stored in your device? Where? How?**

### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

**Describe what you did here.**

### 3. Build your light!

**Make a video showing off your Frankenlight.**

**Include any schematics or photos in your lab write-up.**
