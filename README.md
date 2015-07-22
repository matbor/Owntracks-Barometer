# Owntracks-Barometer

Quick example of what is possible when using [owntracks][2] for iOS, an [mqtt broker][3] with websockets enabled and the new pressure reading value.

This webpage subscribes to the owntracks topic ```owntracks/username/devicename``` and waits for a message [payload][1] in JSON format.

When it recieves the ```p``` value which is the barometric pressure in kPa (kilo Pascal) it converts it to hPa (hectopascals)and plots it on the gauge.

The values are at the altitude of the reading, not at sea level, I haven't added that feature.  This was just a quick example of something you can do with Owntracks.

All settings: mqtt broker, port and topic are set in baro.htm

![](https://raw.githubusercontent.com/matbor/Owntracks-Barometer/master/screenshot.png)

[1]: http://owntracks.org/booklet/tech/json/#_typelocation
[2]: http://owntracks.org
[3]: http://mosquitto.org
