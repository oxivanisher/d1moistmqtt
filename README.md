# d1moistmqtt
Use a Wemos D1 mini with a [capacitive moist sensor](https://www.dfrobot.com/product-1385.html) to monitor your plants soil moisture and put the value into mqtt. It will produce a value between 0 and 100, where 0 is "no water" and 100 is very wet.

## Calibration
You have to calibrate your sensor. Please follow [this guide](https://wiki.dfrobot.com/Capacitive_Soil_Moisture_Sensor_SKU_SEN0193) or enable the `DEBUG` switch and request measurements over MQTT, which will then be printed out on serial, to do so.
Use the corresponding values for `DRY` and `WET` in `config.h` to compile the code and get correct measurements.

## Wireing
| Moist sensor | Wemos D1 mini |
|--------------|---------------|
| OUTPUT       | A0            |
| GND          | G             |
| VCC          | 5V            |
