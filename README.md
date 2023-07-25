# Air Quality Sensor

The purose of this project is to create a stand-alone sensor device for indoor cature of air quality metrics that are displayed on the eInk screen on the device as well as report measurements to Home Assistant.   

Sensor Metrics:
- Temperature
- Humidity
- PM1, PM2.5, PM4, PM10
- VOC
- NOx
- CO2

# Battery Monitoring

[C++ Battery Monitoring Example](https://forum.seeedstudio.com/t/battery-voltage-monitor-and-ad-conversion-for-xiao-esp32c/267535)

```c++
// attenuation ratio 1/2, mV --> V
float Vbattf = 2 * Vbatt / 16 / 1000.0;     
```

# Outside AQI Sensing

Leveraging a commercial / government sensor for outside sensing of AQI on PM2.5 is the ideal configuration.  AirNow.gov has a API which Home Assistant has a integration created to pull in the sensor data.

You must first get a API key here:
https://docs.airnowapi.org/

# Proof of Concept v1


![poc_v1_top](attachments/poc_v1_top.png)

![poc_v1_side](attachments/poc_v1_side.png)
