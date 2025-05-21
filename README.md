# crop-monitoring-and-pest-management
Working Procedure

1. Sensor Data Simulation (Wokwi)
   💠  Simulate the following sensors using Wokwi:
   💠 `DHT22` for temperature and humidity
   💠 `Potentiometer` for soil moisture
   💠 `Button` as a rain sensor
   💠 `Buzzer` and `LED` for pest alert
   💠  Use an OLED display to show sensor readings in real-time.

2. Sensor Data Collection
   💠 Values from the sensors (simulated in Wokwi) are read in the code.
   💠 These include:
   💠 Temperature (°C)
   💠 Humidity (%)
   💠 Soil Moisture (%)
   💠 Rain Detected (Yes/No)

3. Data Transmission (Software-Based Simulation)
   💠 Since the project is software-based, sensor values are either stored in a `.json` file or accessed directly through the backend code (`app.py`).
   💠 No physical ESP32 or Wi-Fi module is used.

4. Backend Processing (Python Flask)
   💠 The `app.py` file reads the sensor data.
   💠 Based on predefined thresholds, it:
   💠 Suggests suitable crops (e.g., rice, wheat, maize)
   💠 Triggers pest alerts if humidity is high or moisture conditions are ideal for pests

5. Website Display (Frontend)
   💠 The frontend (`index.html`, `script.js`) fetches data from the backend.
   💠 Displays:
   💠 Live sensor values
   💠 Suggested crops
   💠 Pest alerts (with buzzer and LED simulated visually)

6. Notification Logic
   💠 If pest-prone weather is detected:
   💠 A buzzer is activated (simulated)
   💠 LED turns on (simulated)
   💠 A red alert is shown on the website
   💠 If all conditions are normal:
   💠 A green message is displayed: "Crops are safe"

7. Final Output
   💠 Users can monitor weather, soil, and pest risk from a single dashboard.
   💠 Helps in early pest management and better crop planning.
