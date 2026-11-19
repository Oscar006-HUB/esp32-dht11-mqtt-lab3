# ESP32 DHT11 → MQTT (Lab 3)

ESP32 sketch that reads temperature and humidity from a DHT11 sensor and publishes the readings to an MQTT broker.

## Contents

| Path | Description |
|------|-------------|
| `labs3/labs3.ino` | ESP32 firmware: WiFi connect, DHT11 read, MQTT publish |
| `Lab 2.jpg`, `lab2 code.jpg` | Photos of the circuit and code |
| `serial monitor.jpg` | Serial monitor output from a test run |

## Hardware

- ESP32 development board
- DHT11 temperature & humidity sensor (data pin → GPIO 4)

## Libraries

- `WiFi.h` (ESP32 core)
- [PubSubClient](https://github.com/knolleary/pubsubclient)
- [DHT sensor library](https://github.com/adafruit/DHT-sensor-library)

## Configuration

WiFi credentials are **not** committed. Before flashing, replace the placeholders in the sketch:

```cpp
const char* ssid     = "YOUR_WIFI_SSID";
const char* password = "YOUR_WIFI_PASSWORD";
```

Also set `mqtt_server` to the IP address of the machine running your MQTT broker.

---

Author: **Prince Oscar Mwinnuo** ([@Oscar006-HUB](https://github.com/Oscar006-HUB))
