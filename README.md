# Easy way to the neuroscience world with the shield for Raspberry Pi. Open-source.   

## To Buy -  PiEEG is available in the market in our partner shop [Elecrow](https://www.elecrow.com/pieeg.html)
  
  
  
  
[Linkedin for updates ](https://www.linkedin.com/company/96475004/admin/feed/posts/) (Not medical device)

[![Software demonstrations](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/Supplementary%20files/fig19.bmp)](https://www.crowdsupply.com/hackerbci/pieeg)     
#### It is not a medical device!!! And can not be used for any medical purposes!!!


#### Power supply - only battery 5V, please read datasheet!!!!!  
#### You are fully responsible for your personal decision to purchase this device and, ultimately, for its safe use. PiEEG is not a medical device and has not been certified by any government regulatory agency for use with the human body. Use it at your own risk.  


#

#

#





This project is the result of several years of work on the development of BCI. We believe that the easiest way to get started with biosignals is to use a shield.
We will try to reveal the process of reading EEG signals as fully and clearly as possible.  [Crowdsupply](https://www.crowdsupply.com/hackerbci/pieeg)

[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=DIY%20Brain-Computer%20%20interface%20PIEEG%20&url=https://github.com/Ildaron/EEGwithRaspberryPI&hashtags=RaspberryPI,EEG,python,opensource)

![alt tag](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/Supplementary%20files/fig.15...jpg "general view")​
-  [Warning](https://github.com/Ildaron/EEGwithRaspberryPI#warning)
-  [How it Works](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/README.md#how-it-works)
-  [Noise measure](https://github.com/Ildaron/EEGwithRaspberryPI#noise-measure)
-  [Device pinout](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/README.md#device-pinout)   
-  [Description of code](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/README.md#description-of-code)
-  [Video-hardware and signal processing demonstration](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/README.md#video---hardware-and-signal-processing-demonstration) 
-  [For beginners](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/README.md#for-beginners)        
-  [Citation](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/README.md#citation)   
-  [Contacts](https://github.com/Ildaron/EEGwithRaspberryPI#contacts)  

#### Warning 
The device must operate only from a battery - 5 V. Complete isolation from the mains power.! The device MUST not be connected to any kind of mains power, via USB or otherwise   

#### How it Works   
 [1.1.Read_data.c](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/1.1.Read_data.c) C script for read data in real-time and save to txt file  
 [1.2.Read_data.cpp](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/1.2.Read_data.cpp) C++ script for read data in real-time and save to txt file   
 [real_time.py](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/GUI/real_time.py) GUI python script for read data in real-time    
 [robot_control.py](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/Robot_control/robot_control.py) script to control a robot by blinking  




Connect the shield to Raspberry PI 3 or RaspberryPI4 and after that connect the device to a battery (power supply) and connect electrodes.
Full galvanic isolation from mains required.  
This also applies to the monitor. Use only a monitor that is powered by the RaspberryPI, as in the picture below, left. Electrodes positioned according to International 10-20 system, right.    
![alt tag](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/Supplementary%20files/fig.7.bmp "general view")​

#### Device pinout  
Shiled connceted with raspbberryPI only in the netxt points     
  43  +5V  
  44  GND  
  37  MOSI  
  34  MISO  
  35  CLKL  
  36  CS  

  
#### Description of the code  
Python script dont allow reading data from ADS1299 with the frequency of 250 Hz. Necessary to use .c or .cpp scripts for reading data in real-time and python for signal processing and vialuzation.   
 


#### Video - Control robot toy by with blinking  
[![Software demonstrations](https://github.com/Ildaron/EEGwithRaspberryPI/blob/master/Supplementary%20files/fig.18.jpg)](https://youtu.be/wNgCEKIXGUY)      


#### For beginners
During the measurement, in addition to artifacts caused by muscle activity, be concerned about the increased resistance between the body and the floor. For example, in the picture below, the moment when the feet touch the floor with and without an insulated shoe. Without insulated shoes - increased noise is noticeable




#### Citation  
I. Rakhmatuiln, M. Zhanikeev and A. Parfenov, "Raspberry PI Shield - for measure EEG (PIEEG)," 2021 5th International Conference on Electrical, Electronics, Communication, Computer Technologies and Optimization Techniques (ICEECCOT), 2021, pp. 410-413, DOI: 10.1109/ICEECCOT52851.2021.9707969  


Rakhmatulin, I., Volkl, S. (2020). PIEEG: Turn a Raspberry Pi into a Brain-Computer-Interface to measure biosignals. arXiv:2201.02228, https://arxiv.org/abs/2201.02228  

#### Contacts  
[Crowdsupply](https://www.crowdsupply.com/hackerbci/pieeg)  
ildarr2016@gmail.com  
http://pieeg.com/
