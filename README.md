This code defines and reads values from three analog sensors connected to an Arduino or compatible board:

GAS_SENSOR: Analog input for a gas sensor (e.g., MQ series).

TEMP_SENSOR: Analog input for a temperature sensor (e.g., LM35 or similar).

SENSOR_3: A third analog sensor input, customizable based on project requirements.


The SensorData struct is used to neatly package sensor readings. The readSensors() function reads the current values of all three sensors using analogRead() and returns them in a SensorData structure.
