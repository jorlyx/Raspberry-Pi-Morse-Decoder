# Raspberry-Pi-Morse-Decoder
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
Overview
This project is an interactive Morse Code Decoder built using a Raspberry Pi and various hardware components including an LED, buzzer, rotary knob, button, and an LCD screen. I completed this in my First Year of Uni, because the code may be used for future coursework i cannot upload it.

The system allows a user to input Morse code using a single button — short presses for dots (.) and long holds for dashes (-). The Raspberry Pi interprets the signal timing, decodes the input, provides both visual and audio feedback, and displays the decoded characters on screen.

 
Features
• Morse Code Input:
o Short press → Dot (.)
o Long hold → Dash (-)
• Real-Time Feedback:
o Short buzz = Dot
o Long buzz = Dash
o Good buzz = Valid Morse sequence
o Bad buzz = Invalid sequence
• Adaptive Input Timing:
o The rotary knob adjusts the timing threshold between a short press (dot) and a long press (dash).
• Visual Output:
o After every correctly decoded letter, it is shown on the LCD display.
• Success/Failure Indicators:
o If all letters are decoded correctly:
▪ LED flashes green
▪ Buzzer plays a victory tune
o If decoding fails:
▪ LED flashes red
▪ Failure tone is played
 
Hardware Components
Component
Purpose
Raspberry Pi
Central controller
LED
Visual status feedback (success/failure)
Buzzer
Audio feedback for dots, dashes, and outcomes
Button
Morse code input device
Rotary Knob
Adjusts timing threshold between press and hold
LCD Screen
Displays decoded characters and final output
 
How It Works
1. The user inputs Morse code using the button.
2. The Raspberry Pi measures how long the button is pressed:
a. Below the threshold → Dot
b. Above the threshold → Dash
3. The buzzer provides immediate feedback for each input.
4. Once a valid Morse letter is entered, it’s decoded using a pre-defined Morse code dictionary.
5. The decoded letter appears on the LCD.
6. After four correct letters in a row, the system checks if the full message is correct and plays either a victory or failure sequence.
 
Skills Demonstrated
• Hardware interfacing using Raspberry Pi GPIO
• Real-time input handling and signal timing
• Embedded systems programming (Python/C depending on implementation)
• Use of dictionaries/mappings for Morse code decoding
• Visual and auditory feedback design
• Integration of multiple I/O components
 
Possible Improvements
• Add serial communication for logging decoded messages to a computer
• Implement adjustable playback speed or learning mode
• Add multi-word message recognition and scoring system
 
Team
Lead my Group in developing a university embedded systems, the team wss passionate about combining electronics and programming to create interactive learning tools.

 
