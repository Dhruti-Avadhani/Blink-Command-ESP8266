# Blink-Command-ESP8266
This was the first Activity Set in my second workshop conducted as a part of my subject, Engineering Explorations. I have given a step by step guide in this repo as to how I was able to blink the built-in led on ESP8266 Microcontroller, and so can you!
<br><br>
I strongly suggest the viewers to go through this README.md file to effectively understand the process to blink the led on the ESP8266 Microcontroller.
<br><br>

<h1>ALL ABOUT ESP8266</h1>
<br>
<p>The ESP8266 is a low-cost Wi-Fi microchip with full TCP/IP stack and microcontroller capability, produced by Shanghai-based Chinese manufacturer Espressif Systems. It's popular among hobbyists and makers due to its affordability, ease of use, and robust community support. Here's a breakdown of the ESP8266 and its connection with NodeMCU:</p>
<br>
<h2>ESP8266 Features:</h2>
<br>
<p>Wi-Fi Connectivity: The ESP8266 provides Wi-Fi connectivity, allowing devices to connect to Wi-Fi networks and communicate with other devices or servers over the internet.</p>
<br>
<p>Microcontroller Capability: Despite being primarily a Wi-Fi module, the ESP8266 also integrates a powerful 32-bit microcontroller, which allows it to execute user code and interact with various sensors, actuators, and other electronic components.</p>
<br>
<p>Low Cost: One of the key attractions of the ESP8266 is its low cost, making it accessible to a wide range of users for various IoT and embedded projects.</p>
<br>
<p>Community Support: There is a large and active community of developers and enthusiasts who have contributed to the development of libraries, tutorials, and projects based on the ESP8266, providing ample resources for newcomers to get started.</p>
<br><br>
<h1>ALL ABOUT NODEMCU</h1>
<br>
<p>NodeMCU is an open-source firmware and development kit that helps you to prototype your IoT product with the ESP8266. It includes firmware that runs on the ESP8266 Wi-Fi SoC from Espressif Systems, and hardware which is based on the ESP-12 module.</p>
<br>
<h2>Connection with NodeMCU:</h2>
<p>Hardware Setup:

NodeMCU boards usually have the ESP8266 chip integrated onto them. They often come with a USB interface for easy programming and power supply.
NodeMCU boards typically have GPIO pins broken out, allowing you to connect sensors, actuators, and other components directly to them.
To connect peripherals to the NodeMCU, you typically use jumper wires. These are small wires that can be connected to the GPIO pins on the NodeMCU and then attached to other components as needed.</p>
<br>
<p>Software Development:

NodeMCU is programmed using the Arduino IDE or Lua programming language. The Arduino IDE is a popular choice due to its ease of use and vast community support.
To program the NodeMCU, you first need to install the ESP8266 board support package in the Arduino IDE, as mentioned earlier.
Once you have the board support package installed, you can select the NodeMCU board from the Arduino IDE's board menu and start writing and uploading code to it.</p>
<br>
<p>Programming:

You write code for the NodeMCU similarly to how you would write code for any other Arduino-compatible board. You can use libraries and functions provided by the Arduino ecosystem to interact with sensors, actuators, and other peripherals connected to the NodeMCU.
The ESP8266 chip has its own set of APIs for Wi-Fi connectivity and other features, which you can also use in your NodeMCU projects.</p>





<br>
<br>

<p>Now let us take a look at a step by step process on how to achieve this blink function on ESP8266</p>
<h1>Arduino IDE Setup</h1>
<br>
<h3>Step 1 : Setup the Arduino IDE to make it compatible to work with ESP8266</h3>
<br>
<p>1. Go to "file" and select "preferences"</p><br>
<p>2. Under "preferences" type the following line into the "Additional Boards Manager URLs"</p><br>
<p>http://arduino.esp8266.com/stable/package_esp8266com_index.json</p><br>
<p>3. Click "OK" to save changes</p><br>
<p>4. Go to "Tools" select "Boards" and navigate to "Boards Manager"</p><br>
<p>5. Search for "ESP8266" and install the library</p><br>
<p>6. Once the installation is complete, restart your ARDUINO IDE</p><br>
<p>7. Once you have reopened Arduino IDE, navigate to "Tools" > "Boards" > "esp8266" > "Node MCU 1.0 (ESP-12E Module)"</p><br>
<p>You may also choose "Node MCU 0.9 (ESP-12 Module)" depending on the options available in your IDE</p><br>
<p>8. Next Plug in the USB to Micro USB cable to your computer device and select the required port from where you will export your code into ESP8266</p>

<h1>Fetching the Code</h1>
<br>
<h3>Step 2 : Fetch the code from Arduino IDE</h3>
<br>
<p>1. The easiest way to get basic codes is to navigate to "File" > "Examples" > "Basics" > "Blink"</p>
<br>
<p>specifically to get the blink command</p><br>
<p>2. Next, we upload the sketch to ESP8266. Simply connect your microcontroller to your computer device using a USB to micro USB cable and select "Upload" to upload the sketch to the microcontroller</p>
<br>
<p>3. After a quick build, the sketch would successfully be uploaded to the microcontroller and you see the LED blink.</p><br>

<h2>or, you can also simply download the file from this repo and use it :)</h2>

<br>
<br>

<h1>Challenges Faced : </h1>
<br>
<p>One challenge that you might face is, if you do not have the 2102 driver installed and running in your computer device, then what typically happens is, the port from which you want to export your file becomes undetectable by the IDE. Here is a quick 2-step guide to help you with this problem</p>
<br>
<p>1. Install the Universal Windows 210x Driver from https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads if you are using a windows machine.</p>
<br>
<p>2. Extract all the files and update settings in your device manager and you are good to go!</p>


















