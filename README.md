# Soumya-Havale

Industrial Health Monitoring System Using IOT System



The ESP32 IoT-Based 3-Phase Induction Motor Monitoring and Protection System is designed to monitor the operating condition of an industrial motor in real time. It measures important parameters such as voltage, current, temperature, and vibration to identify abnormal operating conditions.
The system uses an ESP32 microcontroller to collect sensor readings and send the data to the ThingSpeak IoT platform. A web-based dashboard displays the readings, gauges, historical graphs, and motor status. The system can also detect faults and provide alerts.

*THE MAIN WORKING OF CODE:

1)HTML — Structure of the Dashboard
HTML creates the basic structure of the webpage. In this project, it defines the dashboard title, sensor cards, gauges, graphs, warning banner, and motor-status indicators.
Examples from code:
<h1> displays the dashboard heading.
<div id="gauges"> holds the sensor gauges.
<div id="lamps"> holds the status lights.
<div id="charts"> holds the historical graphs.
<p id="updated"> displays the last update time.
  
2)CSS — Design and Appearance
CSS makes the dashboard attractive and easy to read. It controls the background, card layout, text, colors, status lights, and warning animations.
Examples from code:
.card styles each sensor card.
.grid arranges the cards.
.dot.green displays a green status light.
.dot.red displays a red status light.
.banner.bad highlights a fault warning.
@keyframes blink makes the warning banner blink.

3)JavaScript — Logic and Data Processing
JavaScript makes the dashboard dynamic. It fetches sensor readings from ThingSpeak, extracts values, updates gauges and graphs, checks status fields, and displays fault messages.
Examples from code:
fetch(url) requests data from ThingSpeak.
res.json() converts the response into usable JavaScript data.
update() refreshes the dashboard data.
drawChart() draws the sensor-history graphs.
setInterval(update, REFRESH_MS) repeats the update every 15 seconds.

<img width="1024" height="1536" alt="how the system works" src="https://github.com/user-attachments/assets/64de22e4-fdeb-4088-956b-acf88ab81e11" />

*How to run your dashboard
Open your machine dashboard.html file in VS Code.
Find YOUR_CHANNEL_ID in the JavaScript section and replace it with your ThingSpeak Channel ID.
Add the Read API Key if your ThingSpeak channel is private.
Save the file.
Open it in a browser, preferably using the VS Code Live Server extension.
Connect the ESP32 to Wi-Fi and upload firmware that sends readings to the same ThingSpeak channel.
Check that the readings appear on the dashboard.

<img width="1525" height="728" alt="Dashboard" src="https://github.com/user-attachments/assets/0a288b1f-44e4-403b-b3f6-d2de27a5f812" />


