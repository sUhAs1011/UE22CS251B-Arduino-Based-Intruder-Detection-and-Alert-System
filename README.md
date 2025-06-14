# ALARM-BURGLAR-SYSTEM

### Overview
An alarm burglar system is a security device designed to detect unauthorized entry into a property and alert the owner or security personnel. Using Arduino, such systems can be easily developed, combining sensors, actuators, and communication modules for effective intrusion detection and alert mechanisms

We have used CPP programming language to detect motion using ultrasonic sensor  and respond by turning on a red LED, activating a buzzer, and making a phone call using a GSM module connected via SoftwareSerial.
### Steps for setting up the alarm system
To connect an Arduino to a laptop, you typically follow these steps:

1. *Install Arduino IDE (Integrated Development Environment)*: If you haven't already, download and install the Arduino IDE from the official Arduino website. This software allows you to write, compile, and upload code to your Arduino board.

2. *Connect Arduino to Laptop via USB Cable*: Use a USB cable to connect your Arduino board to one of the USB ports on your laptop. 

3. *Install Drivers (if necessary)*: Most modern operating systems (Windows, macOS, Linux) will automatically recognize the Arduino board and install the necessary drivers. However, if your laptop doesn't recognize the Arduino board, you may need to install the drivers manually. You can usually find the drivers on the Arduino website or included with the Arduino IDE.

4. *Select the Correct Board and Port in Arduino IDE*: Open the Arduino IDE on your laptop. In the IDE, go to the "Tools" menu and select "Board." Choose the correct Arduino board that you're using (e.g., Arduino Uno, Arduino Nano, etc.). Then, go to the "Tools" menu again, select "Port," and choose the port to which your Arduino is connected. On Windows, it may appear as COMx (x being a number), and on macOS, it usually appears as something like /dev/cu.usbmodemXXXX.

5. *Upload a Sketch (Code)*: Now that your Arduino is connected and the correct board and port are selected, you can upload a sketch (code) to your Arduino. You can either write your own code or use one of the many example sketches available in the Arduino IDE. Once you have your code ready, click the "Upload" button (the right arrow icon) in the Arduino IDE. The IDE will compile your code and upload it to the Arduino board.

6. *Monitor Serial Output (Optional)*: If your Arduino sketch includes serial communication, you can monitor the output using the Serial Monitor feature in the Arduino IDE. Go to the "Tools" menu, select "Serial Monitor," and a window will open where you can view the data being sent and received by your Arduino.



Please feel free to update or make any changes in code and you can deploy the project according to yuor requirements and the arduino components you have and please ensure that when you are deploying the code in CPP programming language ensure that you use the module "#include <SoftwareSerial.h>" which allows you to use communication ports on Arduino boards that have only one hardware serial port like arduino uno

Before deploying the code ensure that you have downloaded and installed arduino ide on your computer as the module "#include <SoftwareSerial.h>" can't be run without it  

### Team Members:  
- Sumukh GS (PES2UG22CS596)  
- Suhas Venkata Karamalaputti (PES2UG22CS590)  
- Soham Praveen Salunke (PES2UG22CS565)


![image](https://github.com/user-attachments/assets/dcdf40c5-7555-42fd-929e-a0a8ba7b8941)




