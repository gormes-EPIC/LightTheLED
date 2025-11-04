# Light the LED

## Objective 

1. Build a circuit using a breadboard
2. Calculate the appropriate resistor using Ohm's Law
3. Write a Python script to light an LED using the Raspberry Pi's GPIO pins

## You Will Need

![IMG_2034|400](https://github.com/user-attachments/assets/72bccbd5-edb2-49a8-8b7d-b274788156dd)

- Raspberry Pi
- Breadboard and T-Cobbler
- A resistor (see steps for which resistor)
- LED light (two prongs, any color) 
- Male-to-Male Jumper wires

## Resources You Will Need

- https://gpiozero.readthedocs.io/en/latest/recipes.html#led

## Your Task: Complete Survival Mode or Hardcore Mode


https://github.com/user-attachments/assets/527c8a38-957d-4aa5-ac06-ae0c03985eba


1. **Survival Mode** is best for students who are new to Raspberry Pis and circuits. This is the best fit for most students. 
2. **Hardcore Mode** is best for students who are already familiar with Raspberry Pi's or have taken Introduction to Electronics at EPIC before.


![image001-1](https://github.com/user-attachments/assets/67ed7734-2ac5-4205-9a34-e834d6af0bc8)

## Getting Started: Survival Mode

1. For this project, you will use Python to light an LED with your Raspberry Pi.
2. First you will determine which resistor using **Ohm's Law**. Ohm's law states $V = IR$.
	1. $V$ represents **voltage** and is measured in volts($V$). $I$ represents **current** and is measured in amps($A$). $R$ represents **resistance** and is measured in Ohms($\Omega$).
	2. We trying to solve for required resistance(which we will apply with a resistor), so reorganize the function to solve for resistance. 
	3. Next, the voltage through the function is equal to $V_{supply} - V_{forward}$. Replace $V$ in the function with  $V_{supply} - V_{forward}$.
	4. The $V_{supply}$ provided by the GPIO pins is 3.3V. 
	5. Research 5mm LED's to find their forward voltage and safe current on Sparkfun.
 	6. We only want about half of the maximum current to be applied to the LED, so half your safe current value.
    7. Then plug the values into your function. Remember to convert to volts and amps!
	8. Solve for resistance to find the required resistor. You must select a resistor with **the resistance you solved for or greater** or your LED will explode. 
	9. Check your work with Ormes before moving forward.
3. **Use the above resource** to build your circuit. Connect the light to pin 18. It should look like the picture below.
	- **Warning!** The following could permanently damage your Pi if you do not heed the warnings below.
		- Turn off your Pi when connecting cables to the GPIO ports.
		- Use a resistor, the LED will consumer as much voltage as it can (and explode!). This may damage your Pi, you or your classmates.
		- Do not bend the GPIO pins. Once placing your T-Cobbler onto the Pi, you should not remove it.
	- ![Screenshot from 2024-11-17 13-23-48](https://github.com/user-attachments/assets/c71945e4-6e6b-4d4d-b5fb-ae7357abd337)
4. Open the folder you created during the last lab and create a new file `light.py`. Use the resources above to write a program to turn on pin 18 (which should turn on your light, if wired correctly). Your program should turn the light on, wait a few seconds, then turn the light off.
5. When you are done, take a video of your LED lighting up. Then upload your video and your code to GitHub. 

- [ ] Upload your video and your code to GitHub

![image009-1](https://github.com/user-attachments/assets/80044f9f-7750-4378-855d-9e691fe465b3)

## Getting Started: Hardcore Mode

1. For this project, you will use **Python and the terminal** to light an LED with your Raspberry Pi.
2. First you will determine which resistor using **Ohm's Law**. Ohm's law states $V = IR$.
	1. $V$ represents **voltage** and is measured in volts($V$). $I$ represents **current** and is measured in amps($A$). $R$ represents **resistance** and is measured in Ohms($\Omega$).
	2. We trying to solve for required resistance(which we will apply with a resistor), so reorganize the function to solve for resistance. 
	3. Next, the voltage through the function is equal to $V_{supply} - V_{forward}$. Replace $V$ in the function with  $V_{supply} - V_{forward}$.
	4. The $V_{supply}$ provided by the GPIO pins is 3.3V. 
	5. Research 5mm LED's to find their forward voltage and safe current on Sparkfun.
 	6. We only want about half of the maximum current to be applied to the LED, so half your safe current value.
    7. Then plug the values into your function. Remember to convert to volts and amps!
	6. Solve for resistance to find the required resistor. You must select a resistor with **the resistance you solved for or greater** or your LED will explode. 
	7. Check your work with Ormes before moving forward.
3. Use the above resource, to build your circuit. Connect the light to pin 18. It should look like the picture below.
	- **Warning!** The following could permanently damage your Pi if you do not heed the warnings below.
		- Turn off your Pi when connecting cables to the GPIO ports.
		- Use a resistor, the LED will consumer as much voltage as it can (and explode!). This may damage your Pi, you or your classmates.
		- Do not bend the GPIO pins. Once placing your T-Cobbler onto the Pi, you should not remove it.
	- ![Screenshot from 2024-11-17 13-23-48](https://github.com/user-attachments/assets/c71945e4-6e6b-4d4d-b5fb-ae7357abd337)
4. Open the folder you created during the last lab and create a new file `light.py`. Use the resources above to write a program to turn on pin 18 (which should turn on your light, if wired correctly). Your program should turn the light on, wait a few seconds, then turn the light off.
5. When you are done, take a video of your LED lighting up. Then upload your video and your code to GitHub. 
6. Then, figure out how to use the **terminal only** to light the LED. Add the instructions to do so to your GitHub README. See the resources below for additional help. 

- [ ] Upload your video and your code to GitHub

## Deliverables

- Upload a video of your working project to GitHub
- Upload your code to GitHub
- Mark the assignment as done on Google Classroom
- Answer the following questions either in person or in a written format:  
	- What is the purpose of breadboard? 
	- Does the LED orientation matter (cathode & abode)? 
	- Why do you put a resistor in your circuit?
	- How will a resistor with greater resistance affect the light?

## Additional Resources

- https://embeddedcomputing.com/technology/processing/interface-io/quick-start-raspberry-pi-gpio-terminal-interface # Controlling GPIO with terminal

## Rubric

- 6 points - All required items are present.    
- 5 points - Task was completed, but supplementary materials are weak or missing.    
  - PDF is complete, but poorly communicates necessary information
- 4 points - Task was attempted, but is missing major components.    
  - Missing PDF description or reflection questions  
- 3 points - Did not attempt or student should reattempt.  
  
## Additional Extensions

- Create and document a circuit to control an RGB lightbulb(4 prong).
- Create and document how to SSH intro your Raspberry Pi and activate the lightbulb.
- Expand your Python program to add the library ```time``` or take Terminal input.
- Install Visual Studio code on your Raspberry Pi using ```sudo apt install code```. Then connect your GitHub Account and upload your code.

