# simple_heater_control
This is a simple embedded simulation project that controls a heater (represented by a relay) based on temperature readings using the hysteresis approach to avoid frequent ON/OFF toggling.

📌 How It Works
A DHT22 sensor reads the ambient temperature.

A relay module is used to simulate the heater.

The system turns the heater ON when temperature falls below 24°C.

It turns the heater OFF when temperature rises above 26°C.

If the temperature is between 24°C and 26°C, the system maintains the current heater state (no switching).

This is a classic hysteresis control logic, often used in thermostats to ensure system stability.

🛠️ Components Used
DHT22 Temperature & Humidity Sensor

Relay Module (simulating the heater)

Arduino Uno (Wokwi simulator)

LED (optional, for relay output indication)

🧠 Why Hysteresis?
Without hysteresis, the relay could toggle rapidly if the temperature hovers around a single threshold (e.g., 25°C). Hysteresis adds a buffer zone to avoid such instability.

💻 Simulation
This project is built and tested on Wokwi Simulator, allowing anyone to try it without physical hardware.

📷 Visual

(Simple decision logic used in this project)

🚀 Getting Started
Clone this project or open in Wokwi.

Upload the code to the Arduino.

Adjust the virtual DHT22 temperature to see the relay response.

Modify threshold values if needed.

