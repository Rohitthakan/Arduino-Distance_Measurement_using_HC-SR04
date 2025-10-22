# Arduino-Distance_Measurement_using_HC-SR04


This project uses an Arduino microcontroller with an HC-SR04 ultrasonic sensor to measure distances. The Arduino emits ultrasonic pulses and measures the time it takes for the echo to return. This time-of-flight measurement is converted into distance using basic physics. The project demonstrates real-time signal acquisition, instrumentation, and basic data processing.

# Key Components:

## Hardware

- Arduino Uno/Nano: Controls the sensor and collects echo timings.

- HC-SR04 Ultrasonic Sensor: Emits sound waves and measures their return.

- Connecting wires and breadboard.

## Software

- Arduino IDE sketch: Generates trigger signals, reads echo pulses, calculates distances.

- Optional Python script: Reads data from Arduino over serial, filters noise, logs readings, and performs basic analysis.

## Technical Details:

- Signal Acquisition: The Arduino triggers a 40kHz ultrasonic pulse. When the echo returns, it measures the pulse width using the Arduino’s digital I/O pins.

- Distance Calculation: Distance is calculated as:

Distance = (Time-of-flight × Speed of Sound)/2	​

The division by 2 accounts for the round trip of the pulse.

- Data Processing: Measurements can be streamed to a PC for logging or statistical analysis (average, standard deviation, anomaly detection).
