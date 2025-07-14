# **Final Plan for Lesson 11: Embedded Systems & IoT**

### **The Goal**

To create a practical-oriented, single-page A4 cheat sheet for A/L ICT Competency 11, covering the concepts of Embedded Systems and the Internet of Things (IoT). This plan is based on the specific components, code, and methodologies found in both the official syllabus and the government-issued practical resource book.

### **The Structure: "From Component to Global Network"**

This cheat sheet is logically divided into three parts, starting from the fundamental building blocks and progressing to broader concepts and their applications.

## **Cheat Sheet Content**

### **Part 1: "The Thing" \- Embedded Systems & Arduino Fundamentals (Competency Level 11.1)**

*This section focuses on the practical hardware and core programming commands for a single device.*

* **Core Concepts:**  
  * **Embedded System:** A computer system embedded within a larger system (e.g., a washing machine). This is also known as **Physical Computing**.  
  * **IPO Model:** Follows the Input (Sensors) \-\> Process (Microcontroller) \-\> Output (Actuators) model.  
  * **Microcontroller vs. Microprocessor:** A microcontroller is a single chip containing the CPU, memory (RAM, ROM), and I/O ports. In a microprocessor-based system, these are external, separate components.  
  * **IEEE Definition:** A computer system that is part of a larger system and performs some of the requirements of that system.  
* **The Development Board: Arduino Uno**  
  * **Key Features (as per diagram):**  
    * 2: USB Port (for Programming and Power)  
    * 4: Analog Input Pins (A0-A5)  
    * 5: Microcontroller (ATmega328P)  
    * 9: Digital I/O Pins (0-13)  
* **The Software: Arduino IDE**  
  * Arduino programs are called **Sketches**.  
  * **IDE Components:** Verify Button, Upload Button, Code Editor, Console Window.  
* **Firmware Structure & Logic:**  
  * Every Arduino Sketch must have two main functions: void setup() (runs once for initialization) and void loop() (runs over and over again).  
  * An **endless loop** is used because embedded systems do not have an Operating System (OS) to return control to after a program finishes.  
* **Commonly Used Components (Practicals):**  
  * **Outputs:** LED, Piezo Buzzer, DC Motor.  
  * **Inputs:** LDR (Light Dependent Resistor), LM35 Temperature Sensor, Reed Switch.  
  * **Other:**  
    * Resistor (to limit current \- e.g., **220Ω, 10kΩ**)  
    * Transistor (to control high-power devices like motors \- e.g., **BC547**)  
    * Diode (to protect against motor flyback current \- e.g., **1N4001**)

#### **Core Arduino Functions**

* pinMode(pin, MODE); \- Sets a specific pin as an INPUT or OUTPUT.  
* digitalWrite(pin, STATE); \- Sets a digital pin to HIGH (5V) or LOW (0V).  
* digitalRead(pin); \- Reads the state (HIGH or LOW) of a digital pin.  
* analogRead(pin); \- Reads a voltage value (from 0-1023) from an analog pin.  
* delay(ms); \- Pauses the program for a specified number of milliseconds.  
* tone(pin, frequency); \- Generates a sound tone on a specific pin.  
* noTone(pin); \- Stops the tone.  
* Serial.begin(baudRate); \- Starts serial communication with the computer.

### **Part 2: "The Network" \- Practical IoT with Arduino (Competency Level 11.2)**

*This section focuses on the specific hardware and code required to connect an Arduino board to the internet.*

* **Core Concepts:**  
  * **IoT Definition:** A network of interconnected embedded systems that communicate with each other over the Internet.  
  * **Goal:** To create a "Smart World" for convenience and comfort.  
* **Building an IoT Device (Smart Light Example):**  
  * **Key Hardware:** **Arduino Ethernet Shield** \- an add-on module that provides internet connectivity to the Arduino board.  
  * **Important:** When the Ethernet Shield is in use, digital pins 4, 10, 11, 12, and 13 are reserved for it and cannot be used for other purposes.

#### **Core IoT/Ethernet Functions**

* **Library:** \#include \<Ethernet2.h\> must be included at the beginning of the code.  
* **Variables:**  
  * byte mac\[\] \= { 0x.., 0x.. }; \- Holds the unique MAC address of the shield.  
  * EthernetServer server \= EthernetServer(80); \- Creates a server object on port 80 (for HTTP).  
* **In the** setup() **function:**  
  * Ethernet.begin(mac); \- Connects to the network using DHCP.  
  * Serial.println(Ethernet.localIP()); \- Displays the IP address assigned to the device.  
  * server.begin(); \- Starts the web server to listen for clients.  
* **In the** loop() **function:**  
  * EthernetClient client \= server.available(); \- Checks if a client has connected.  
  * client.connected() \- Checks if the client is still connected.  
  * client.read() \- Reads data sent by the client.  
  * client.stop() \- Disconnects the client.

### **Part 3: Applications & Implications**

*A summary of the example systems from the practical book and the social impact of IoT.*

* **Example Systems:**  
  * **Blinker:** Blinks an LED at a regular interval.  
  * **AutoLight:** Controls an LED based on the ambient light intensity from an LDR.  
  * **AutoFan:** Controls a fan motor based on the temperature from an LM35 sensor.  
  * **Door-Alarm:** Triggers a buzzer using a reed switch when a door is opened.  
  * **Smart Light (IoT):** Controls an LED remotely over the internet via HTTP requests.  
* **Social & Security Consequences:**  
  * Social Isolation.  
  * **Security & Privacy:** Risk of unauthorized control of devices and access to personal data.