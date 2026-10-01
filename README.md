# ESP32 Temperature & Humidity Monitoring System

An IoT-based environmental monitoring system using **ESP32**, **DHT22**, and an **I2C 16x2 LCD** to measure and display real-time temperature and humidity data.

## 📌 Overview

The **ESP32 Temperature & Humidity Monitoring System** is designed to monitor environmental conditions using a DHT22 digital sensor.

The ESP32 reads temperature and humidity values from the DHT22 sensor and communicates with an I2C LCD to display the measured data. The complete circuit is developed and tested using the **Wokwi simulation platform**.

## ✨ Features

* Real-time temperature monitoring
* Real-time humidity monitoring
* ESP32-based IoT implementation
* DHT22 digital temperature and humidity sensor
* I2C communication for LCD display
* Serial Monitor support
* Wokwi-based simulation

## 🧰 Technologies & Components

| Category        | Details      |
| --------------- | ------------ |
| Microcontroller | ESP32        |
| Sensor          | DHT22        |
| Display         | I2C 16x2 LCD |
| Programming     | Arduino C++  |
| Simulation      | Wokwi        |

## 🔌 Circuit Connections

| Component | Pin  | ESP32   |
| --------- | ---- | ------- |
| DHT22     | VCC  | 3.3V    |
| DHT22     | DATA | GPIO 4  |
| DHT22     | GND  | GND     |
| LCD       | VCC  | 3.3V    |
| LCD       | GND  | GND     |
| LCD       | SDA  | GPIO 21 |
| LCD       | SCL  | GPIO 22 |

The circuit configuration uses GPIO 4 for DHT22 data and GPIO 21/22 for I2C communication with the LCD.

## ⚙️ Working Principle

```text
       ┌──────────────┐
       │    DHT22     │
       │    Sensor    │
       └──────┬───────┘
              │
       Temperature &
         Humidity
              │
              ▼
       ┌──────────────┐
       │    ESP32     │
       │ Microcontroller│
       └──────┬───────┘
              │
          I2C Data
              │
              ▼
       ┌──────────────┐
       │  I2C LCD     │
       │   Display    │
       └──────────────┘
```

### Process

1. The DHT22 sensor captures temperature and humidity data.
2. The ESP32 reads the sensor values.
3. The ESP32 processes the received data.
4. The values are sent to the I2C LCD.
5. Temperature and humidity readings are displayed on the LCD.
6. The output can also be monitored through the Serial Monitor.

## 📂 Project Structure

```text
ESP32-Temperature-Humidity-Monitoring/
│
├── sketch.ino
├── diagram.json
├── wokwi-project.txt
└── README.md
```

## 🖥️ Simulation

This project is simulated using **Wokwi**, allowing the ESP32 circuit and sensor behavior to be tested virtually.

**Wokwi Project:**
https://wokwi.com/projects/476469838686994433

## 🎯 Applications

This type of monitoring system can be used for:

* Smart home environmental monitoring
* Weather and climate monitoring
* Indoor temperature monitoring
* IoT-based environmental sensing
* Academic and prototype IoT applications

## 🔮 Future Enhancements

The project can be extended with:

* Cloud-based data monitoring
* Mobile application integration
* Wi-Fi-based remote monitoring
* Data logging and historical analysis
* IoT dashboards and alerts

## 📚 Learning Outcomes

Through this project, the following concepts are demonstrated:

* ESP32 programming
* Sensor interfacing
* Temperature and humidity monitoring
* I2C communication
* LCD interfacing
* IoT system development
* Wokwi-based circuit simulation

## 👩‍💻 Author

**Thanalakshmi G**

B.Tech – Computer Science and Business Systems
Ramco Institute of Technology

## 📄 License

This project is created for **educational and learning purposes**.
