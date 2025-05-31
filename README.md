# Sensor-reader
Arduino code to read gas, temperature, and an additional sensor
// Pin definitions for the sensors
#define GAS_SENSOR    A0
#define TEMP_SENSOR   A1
#define SENSOR_3      A2

// Struct to hold sensor readings
struct SensorData {
    int gas;
    int temp;
    int sensor3;
};

// Function to read all sensors and return the data as a struct
SensorData readSensors() {
    SensorData data;
    data.gas = analogRead(GAS_SENSOR);
    data.temp = analogRead(TEMP_SENSOR);
    data.sensor3 = analogRead(SENSOR_3);
    return data;
}
