# 🌐 ESP32 Captive Portal Demo

This project demonstrates how to set up a **captive portal** on an ESP32 using `ESPAsyncWebServer`, `DNSServer`, and `SPIFFS`.  

When a device connects to the ESP32's Wi-Fi access point, it is redirected to a captive portal page (like what you see in airports or hotels). The page contains a demo form where users can enter **test credentials** (SSID/password).  

The ESP32 then tries to connect to the target Wi-Fi network and reports back the connection status.

---

## ✨ Features
- 📡 ESP32 in **Access Point (AP) mode**  
- 🛜 **Captive portal** with DNS redirection  
- 📝 Demo form to collect Wi-Fi credentials (SSID + password)  
- 🔄 Attempts to connect to target Wi-Fi network and shows **success/failure**  
- 💾 Credentials/status stored in **SPIFFS** for review  
- 🎓 Designed as an **educational demo** for IoT provisioning and captive portals  

---

## 🚀 Getting Started

### 1. Requirements
- ESP32 board  
- Arduino IDE or PlatformIO  
- Libraries:  
  - `ESPAsyncWebServer`  
  - `AsyncTCP`  
  - `ArduinoJson`  
  - `DNSServer`  
  - `SPIFFS`  

### 2. Upload SPIFFS files
Upload the provided **`index.html`** to SPIFFS using the Arduino IDE plugin or PlatformIO.

### 3. Flash the sketch
Upload the sketch to your ESP32.  

The ESP32 will create an open Wi-Fi access point:

## ⚠️ Ethical Use

This project is for **educational purposes only**.  
It is designed to demonstrate how captive portals and Wi-Fi provisioning work in IoT devices.  

🚫 It does **not**:  
- Force devices to connect  
- Intercept real user data  
- Perform deauthentication or "evil twin" style attacks  

✅ Always:  
- Use only with devices/networks you control  
- Inform participants that this is a **demo** and only use **test credentials**  
