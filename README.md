# IMU_GY91-WebApp_BLE
This repository contains two web applications built with HTML, CSS, and JavaScript for working with **ESP32 BLE sensor data**.  
Both apps connect to an ESP32 over Bluetooth Low Energy (BLE) and visualize the received packets differently.

---

## 1. IMU GY91 - BLE Data Read - Web Application
This application is designed to display raw BLE packets in multiple formats, making it easier to debug and interpret sensor data.  

It supports:
- **Hexadecimal view** (raw bytes as hex)
- **Binary view** (bit-level representation)
- **IEEE754 decoded floats** (every 4 bytes interpreted as a float)

### Features
- Connect/Disconnect to an ESP32 BLE device  
- Send ON/OFF commands to control an LED  
- View real-time incoming packets in hex, binary, and IEEE754 formats  

### Screenshot
![1](https://github.com/syedmohiuddinzia/IMU_GY91-WebApp_BLE/blob/main/media/1.png)

---

## 2. IMU GY91 - Single Graph - Web Application
This appication extends the BLE data visualization by plotting incoming sensor values as **real-time graphs**.  
It is especially useful for monitoring **IMU (Inertial Measurement Unit)** readings.

### Features
- Connect/Disconnect to an ESP32 BLE device  
- Send ON/OFF commands to control an LED  
- Real-time plotting of IMU sensor data using **Chart.js**  
- Toggle variables (accelerometer, gyroscope, magnetometer, quaternions, Euler angles, temperature, pressure, etc.)  
- Up to 1500 data points stored and displayed  

### Screenshot
![2_1](https://github.com/syedmohiuddinzia/IMU_GY91-WebApp_BLE/blob/main/media/2_1.png)
![2_2](https://github.com/syedmohiuddinzia/IMU_GY91-WebApp_BLE/blob/main/media/2_2.png)

---

## Tech Stack

- **HTML5, CSS3, JavaScript**
- **Web Bluetooth API** for BLE communication
- **Chart.js** for real-time graph plotting
- Responsive UI with a simple **card-based layout**

---

## Usage

1. Open the desired web app in a supported browser (e.g., Chrome).  
2. Click **Connect to BLE Device** and select your ESP32.  
3. Start receiving live sensor data.  
4. Use the controls to view packets or visualize graphs.  

---

## Future Improvements
- Add data export (CSV/JSON)  
- Multi-device support  
- Advanced filtering and scaling options for graphs  
