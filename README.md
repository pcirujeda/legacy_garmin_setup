# Legacy Garmin outdoors GPS setup

My good old [Garmin Etrex Legend H](https://buy.garmin.com/en-US/US/p/30120) was produced in the late 2000s; sports a robust, monochrome, 160 x 288 pixels LCD display; runs on 2 x AA batteries; and holds some -today ridiculous- 24Mb.

Yes, it's discontinued according to today's consumism standards, but it never let me down and it looks it will guide me around for some more years no matter how many trails, rain, mud, wind and dust we collect. That's why I created this little setup tool to keep it functional nowadays, even under Linux as a primary operative system.

The ```install-device``` script is a simple state machine that will allow you to setup your machine to use any Garmin USB gps device, by:

* looking for USB connected Garmin devices
* blacklisting garmin_gps module
* creating udev rules
* blacklisting the GPS from power rules
* installing the necessary system packages