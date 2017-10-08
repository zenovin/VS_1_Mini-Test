# VS_1_Mini-Test
Mini-Test of Assignment 4


1. (Sensor Framework)
Write a small code snippet to show how to perform the following tasks
  * List available sensors on a device
  ``` java
  SensorManager sensorMgr = (SensorManager) getSystemService(SENSOR_SERVICE);
  List<Sensor> sensors = sensorMgr.getSensorList(Sensor.TYPE_ALL);
  ```
  * Retrieve the value range of a specific sensor
  ```java
  sensor.getMaximumRange
  ```
  * Register for monitoring accelerometer sensor changes at the maximum available rate
  ```java
  sensor = sensorMgr.getDefaultSensor(Sensor.TYPE_ACCELEROMETER);
  
  sensorMgr.registerListener(this, sensor, SensorManager.SENSOR_DELAY_FASTEST);
  ```
  
  * ??????????????????
  
2. 
```
onStart() -> onResume() -> RUNNING -> onPause()
onPause() -> PAUSE -> onResume()
??????????
```
3. String values should be defined in a xml file. This offers multiple use of one value (easy to change) and also easier multilanguage support.

4. "An Intent is a messaging object [...]" [https://developer.android.com/...]. Can be used to start Activity, Services or deliver a broadcast. Explicit Intents have to specify the components by name (e.g. class name) and are used inside the own application. Implicit Intents declare general actions to be performed.
5. a) false, b) false???, c) true, d) true??
6.
```xml
<service android:name=".ExampleService" />
```
