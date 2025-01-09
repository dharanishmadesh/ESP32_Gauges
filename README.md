Here’s a **README.md** file for your GitHub repository, formatted for easy understanding and professional presentation:

```markdown
# ESP32 Web Server with Gauges for Real-Time Sensor Readings

This project demonstrates how to create a real-time web server using the **ESP32**, **BME280 sensor**, and **LittleFS**. The web server displays temperature and humidity readings on a dashboard with live updates using server-sent events (SSE).

---

## 🛠 Features

- Real-time temperature and humidity monitoring using the **BME280** sensor.
- Web dashboard with gauges to display sensor data dynamically.
- **LittleFS** integration to serve web content.
- Server-Sent Events (SSE) for live data updates.
- Wi-Fi connectivity for remote monitoring.

---

## 🔧 Components Required

1. ESP32 Development Board
2. BME280 Temperature and Humidity Sensor
3. Jumper Wires
4. Breadboard (Optional)

---

## 📑 Installation and Setup

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/esp32-web-server-gauges.git
cd esp32-web-server-gauges
```

### 2. Install Required Libraries
Ensure you have the following libraries installed in your Arduino IDE:
- **Adafruit BME280 Library**
- **Adafruit Unified Sensor Library**
- **ESPAsyncWebServer**
- **AsyncTCP**
- **Arduino_JSON**

You can install these via the Arduino Library Manager.

### 3. Upload the LittleFS Filesystem
- Install the [LittleFS Plugin](https://randomnerdtutorials.com/install-esp32-filesystem-uploader-arduino-ide/) for your Arduino IDE.
- Copy the `index.html` file (and other assets) to a `data` folder in the project directory.
- Upload the LittleFS filesystem to the ESP32.

### 4. Configure Wi-Fi Credentials
Update the `ssid` and `password` variables in the **main code**:
```cpp
const char* ssid = "REPLACE_WITH_YOUR_SSID";
const char* password = "REPLACE_WITH_YOUR_PASSWORD";
```

### 5. Upload the Code
- Connect your ESP32 to the computer via USB.
- Select the correct board and port in the Arduino IDE.
- Upload the code to the ESP32.

---

## 🖥 Web Dashboard

Once the ESP32 is connected to Wi-Fi, it will display its IP address in the serial monitor. Open this IP address in your browser to access the web dashboard.

---

## 📊 Live Updates

The dashboard automatically updates the sensor readings every 10 seconds using **Server-Sent Events (SSE)**.

---

## 🧰 Circuit Diagram

### BME280 Sensor Connections:
- **VCC** → 3.3V on ESP32
- **GND** → GND on ESP32
- **SDA** → GPIO 21 on ESP32
- **SCL** → GPIO 22 on ESP32

---

## 🧪 Example Output

### Serial Monitor
```plaintext
Connecting to WiFi ...
192.168.1.100
```

### Web Dashboard
- Temperature: 24.5°C
- Humidity: 50%

---

## 📜 License

This project is licensed under the MIT License. See the original [Random Nerd Tutorials](https://randomnerdtutorials.com/esp32-web-server-gauges/) for more details.

---

## 🌟 Acknowledgments

Special thanks to **Rui Santos & Sara Santos** for the original tutorial and inspiration for this project.

---

## 💡 Contribution

Feel free to open issues or submit pull requests for improvements and suggestions. Let’s build something great together!

---

Happy coding! 😊
```

### Key Points:
- Replace `yourusername` with your actual GitHub username in the repository link.
- Add the required `index.html` and other assets to the repository's `data` folder before uploading.

Let me know if you’d like to add more customization or details!
