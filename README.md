# 🌱 Automatic Plant Watering System using ESP32

Sistem penyiraman tanaman otomatis berbasis ESP32 yang mampu memantau kelembapan tanah, suhu, dan kelembapan udara secara real-time. Sistem dapat mengontrol pompa air secara manual melalui Bluetooth maupun melalui jaringan WiFi (sesuai versi program).

---

## Features

- Monitoring soil moisture
- Monitoring temperature and humidity (DHT11)
- Display sensor data on LCD I2C
- Water pump control using relay
- Bluetooth communication (Bluetooth Version)
- WiFi communication (WiFi Version)
- ESP32 as the main controller

---

## Hardware Components

| Component | Quantity |
|-----------|---------:|
| ESP32 Dev Board | 1 |
| Soil Moisture Sensor | 1 |
| DHT11 Temperature & Humidity Sensor | 1 |
| Relay Module 2 Channel | 1 |
| Water Pump DC | 1 |
| LCD I2C 16x2 | 1 |
| Battery / Power Supply | 2 |
| Connecting Wires | Several |

---

## Pin Configuration

| ESP32 Pin | Component |
|-----------|-----------|
| GPIO34 | Soil Moisture Sensor |
| GPIO26 | Relay Module |
| GPIO32 | DHT11 Data |
| GPIO17 | LCD SDA |
| GPIO16 | LCD SCL |

---

## System Workflow

1. ESP32 reads soil moisture.
2. ESP32 reads temperature and humidity from DHT11.
3. Sensor values are displayed on the LCD.
4. Sensor data are sent to the smartphone.
5. The user can turn the water pump ON or OFF remotely.
6. The relay controls the water pump.

---



---

## Required Libraries

Install the following Arduino libraries:

- BluetoothSerial
- Wire
- LiquidCrystal_I2C
- DHT Sensor Library
- Adafruit Unified Sensor

---

## Bluetooth Version

Bluetooth Name

```
SiramTanaman
```

Command

| Command | Function |
|----------|----------|
| 1 | Pump ON |
| 0 | Pump OFF |

The ESP32 continuously sends:

```
Soil: 65%
Temp: 29°C
Humidity: 74%
```

---

## WiFi Version

The WiFi version allows monitoring and controlling the watering system through a wireless network.

---

## Display

LCD displays:

```
Soil: 65%

T:29C H:74%
```

---

## Applications

- Smart Agriculture
- Home Gardening
- Automatic Plant Watering
- IoT Learning Project

---

## Author

**Dio Abiyyu Zidane Ginting**

Informatics Engineering Student

ESP32 • IoT • Embedded Systems • Smart Agriculture
