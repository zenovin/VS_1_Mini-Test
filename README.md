# VS_1_Mini-Test
Mini-Test of Assignment 4

(Sensor Framework) Write a small code snippet to show how to perform the following tasks

  1. List available sensors on a device
  ``` java
  SensorManager sensorMgr = (SensorManager) getSystemService(SENSOR_SERVICE);
  List<Sensor> sensors = sensorMgr.getSensorList(Sensor.TYPE_ALL);
  ```
  2. Retrieve the value range of a specific sensor
  ```java
  sensor.getMaximumRange
  ```
  3. Register for monitoring accelerometer sensor changes at the maximum available rate
  ```java
  sensor = sensorMgr.getDefaultSensor(Sensor.TYPE_ACCELEROMETER);
  
  sensorMgr.registerListener(this, sensor, SensorManager.SENSOR_DELAY_FASTEST);
  ```
  
  
