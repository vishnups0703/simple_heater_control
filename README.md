# 🔥 Simple Heater Control System

This project simulates a simple temperature-controlled heater system using a microcontroller. It demonstrates the use of **hysteresis control** to avoid rapid switching of a relay based on fluctuating temperature readings.
![Simulation](https://github.com/vishnups0703/simple_heater_control/blob/main/linkedin_heater.png?raw=true)


---

## 📌 Objective

- Turn **ON** the heater when the temperature goes **below 24°C**.
- Turn **OFF** the heater when the temperature rises **above 26°C**.
- **Maintain current state** when temperature is between 24°C and 26°C (hysteresis buffer).

---

## ⚙️ Components Used

- Temperature Sensor (DHT22)
- Relay Module
- Microcontroller (Arduino)
- LED (for simulation)


---

## 🔁 Hysteresis Logic

Instead of switching the heater **ON/OFF** at a single threshold (which may cause relay to toggle rapidly due to slight fluctuations), a **buffer zone** is introduced:

IF temperature < 24°C:
Turn ON heater
ELSE IF temperature > 26°C:
Turn OFF heater
ELSE:
Maintain previous heater state

---

## 🧠 Why Hysteresis?

Without hysteresis:
- Rapid temperature changes (±0.1°C) near the threshold could cause **relay chatter** (unwanted rapid switching).

With hysteresis:
- Adds a **safe deadband** between ON and OFF conditions.
- Improves **stability** and **realism**.
- Common in thermostats and industrial control systems.

---




