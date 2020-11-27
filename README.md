# ESP32-SPI  [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)<br>
Some SPI related notes...
 


### Wires to connect SPI SD/TF card <br>
Use ESP32's VSPI , works on Arduino SdFat library<br>
<img src="pic/ESP32-SD.jpg" width=800 /> &nbsp;&nbsp;&nbsp;<br><br>
<img src="pic/SdInfo.jpg" width=400 /> &nbsp;<img src="pic/SdBench.jpg" width=400 /><br><br>
<br>
 - Change SPI pins in SdSpiDriver.h: _SPI.begin(18,19,23); //Change to VSPI_ <br>
 - Change SPI Speed from 50MHz to 25MHz:  _if (!sd.cardBegin(SD_CHIP_SELECT, SD_SCK_MHZ(25))) {   //works under 25MHz_ <br>

<br>
<br>

### References
  - [Arduino SdFat V2](https://github.com/greiman/SdFat) Arduino library SdFat.
