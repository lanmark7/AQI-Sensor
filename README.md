# Air Quality Sensor

The purpose of this project is to create a stand-alone sensor device for indoor capture of air quality metrics that are displayed on the eInk screen on the device as well as report measurements to Home Assistant.  This project was inspired by the various forest fires causing poor AQI as well as local neighbors firepits that can spike indoor air quality.

# Device Details

Sensirion Sen55 Sensor:  ([Datasheet](https://sensirion.com/media/documents/6791EFA0/62A1F68F/Sensirion_Datasheet_Environmental_Node_SEN5x.pdf))
- Temperature
- Humidity
- PM1, PM2.5, PM4, PM10
- VOC
- NOx

NeoPixel LED (WS2812b):
- LED for showing alert status

# Device Design

The case design is built around a small-ish form factor that allows the eInk display to be centered even though the connector placement and the fact it is a side mounted connector makes for a wider case.  The extra width does allow for some decent component placement like a battery pack, processor and core sensor.

![device_front](attachments/device_front.png)

![device_inside](attachments/device_inside.png)

![device_wiring](attachments/device_wiring.png)

# Outside AQI Sensing

Leveraging a commercial / government sensor for outside sensing of AQI on PM2.5 is the ideal configuration.  AirNow.gov has a API which Home Assistant has a integration created to pull in the sensor data.

You must first get a API key here:
https://docs.airnowapi.org/

# Battery Monitoring

I started out attempting to make this sensor battery powered in addition to USB powered, however I just can't get consistent results yet and so the battery monitoring component of this project has been put on hold in favor of a always plugged in design approach.

# Case Design

## Latest Design

After a number of 3D printing and fitting components this design.  This version is the 5th version of the case front and 3rd version of the back.  The back I think needs another revision to give a little bit more room for the SEN55 sensor since it is overly tight.

![poc_v5_front](attachments/poc_v5_front_cover.png)

![poc_v5_back](attachments/poc_v5_back_cover.png)

## First Proof of Concept (aka: v1)

Original first attempt at fitting in the components and getting a feel for size and functionality.

![poc_v1_top](attachments/poc_v1_top.png)

![poc_v1_side](attachments/poc_v1_side.png)
