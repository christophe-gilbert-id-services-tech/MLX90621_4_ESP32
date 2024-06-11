### MLX90621 Arduino and Processing example code : adaptation for ESP32

Arduino and Processing code for the Melexis [MLX90621](http://www.melexis.com/Infrared-Thermometer-Sensors/Infrared-Thermometer-Sensors/Low-noise-high-speed-16x4-Far-Infrared-array-823.aspx) 16x4 thermopile array.

Includes R script to parse data files (which can be exported by Processing visualizer).

The MLX90621 FIRray temperature sensing device from Melexis utilizes the company’s non-contact temperature measurement technology to create a highly cost-effective thermography solution. Covering a -20°C to 300°C temperature range, this 16 x 4 element far infrared (FIR) thermopile sensor array produces a map of heat values for the target area in real time, avoiding the need to scan the area with a single point sensor or use an expensive microbolometer device.

In use in VU and Tilburg University temperature [cry detection project](http://www.pavlov.io/2015/07/01/detecting-crying-eyes/).

Implements MaxBot's MLX90621 [Arduino library](http://forum.arduino.cc/index.php?topic=126244.0) patched with KMoto's [minor change](http://forum.arduino.cc/index.php?topic=126244.msg2307588#msg2307588) in defaultConfig_H.
  Modified for ESP32

TODO 2015-10-25: Refactor and clean up Processing visualizer.
TODO : parameter when starting sensor, to choose I2C port : I2C1 / I2C0 / custom
        Target is to grab multiple sensors on 1 ESP32

##### Screenshot

![](board.png)
![](screenshot.gif)
