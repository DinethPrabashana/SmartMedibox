# Smart Medibox Simulation

## Description

The Smart Medibox is an embedded system designed to assist users in managing their medication schedules and monitoring environmental conditions like temperature and humidity. Developed as part of the EN2853 Embedded Systems and Applications course, this project uses an ESP32 microcontroller to simulate a fully-functional Medibox with a user-friendly interface.

### Key Features:
- **Time Management:** Set time zones and alarms for medication reminders.
- **Alarm System:** Alerts the user with an audible alarm and visual indicators, which can be stopped or disabled.
- **Environmental Monitoring:** Continuously monitors temperature and humidity levels, providing warnings if they exceed healthy limits.

## Procedure

### 1. Set Up the Wokwi Simulation

1. **Create a New Project:**
   - Go to [Wokwi Simulator](https://wokwi.com/).
   - Start a new project and choose the ESP32 microcontroller.

2. **Add Required Components:**
   - **OLED Display:** To display the current time, alarm settings, and environmental data.
   - **Buzzer:** For sounding alarms when medication is due.
   - **DHT22 Sensor:** To monitor temperature and humidity.
   - **Push Button:** To stop or disable the alarms.

3. **Wire the Components:**
   - Connect the OLED display to the appropriate GPIO pins on the ESP32.
   - Wire the buzzer, DHT22 sensor, and push button to their respective pins.

### 2. Programming the ESP32

1. **Write the Code:**
   - Implement the code to handle the following functionalities:
     - **Time Management:** Use Wi-Fi to fetch the current time from an NTP server and adjust it based on the selected time zone.
     - **Alarm System:** Allow users to set, disable, and stop alarms. The alarm should ring at the set time and provide visual feedback on the OLED.
     - **Environmental Monitoring:** Continuously read temperature and humidity data from the DHT22 sensor and display it on the OLED. Trigger warnings if the values exceed the healthy limits.

2. **Upload the Code:**
   - Upload the code to the ESP32 in the Wokwi simulation environment.
   - Test the system by setting different time zones, alarms, and adjusting the temperature/humidity to observe the system's response.

### 3. Testing the System

- **Test Alarm Functionality:** Set alarms at different times and verify that the buzzer and visual indicators function correctly when the alarm triggers.
- **Test Environmental Monitoring:** Simulate various temperature and humidity levels to ensure that warnings are correctly displayed when thresholds are exceeded.
- **Test Menu Navigation:** Ensure that the menu options for setting time zones, alarms, and disabling alarms are easy to navigate and function as expected.



