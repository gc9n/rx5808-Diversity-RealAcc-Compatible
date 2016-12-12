
<h1>OSD Support (Menus-RSSI-Diversity-Battery) Fatshark Button Support</h1>

* Added OSD support for menus
* Ultra fast Real time RSSI feed back
* Ultra fast  Real time Diversity feed back
* PAL or NTSC recognition
* Goggles Battery monitor
* Fatshark Buttons Compatibility
* Favorites enhancement

VIDEO

[![Diversity Module RealAcc with OSD (Real time RSSI-Diversity) and Fatshark button support 
](https://img.youtube.com/vi/VvQDdLFI8oQ/0.jpg)](https://www.youtube.com/watch?v=VvQDdLFI8oQ)

<h1>Powering the module from deferent power source</h1>
 What I realized is that the Fatshark Goggles have an internal regulator 5v that feeds the Video RX module when we plug it in … is less than 500mha. I came to that conclusion because 
RealAcc div module works at 340mha
Microminim OSD works at 100mha
Total 440mha.. The micro minim OSD cannot start combined with the realacc module. 

Plus all those Diversity modules on the market makes our goggles sensitive because  they 
pull as much current as much the glasses can not give . Fatsharks are not designed to give that current , they work  close to the limit!!  . IMHO There is danger if you use diversity modules with the goggles , you pushing them to the limit.

So i made a decision, I didn’t want to open the goggles for any reason, so I had to find a way to power the module from a different power source. With an easy and clean method, without any modifications to the goggles it self.

Then I saw the fan from the face plate! , so I just took power from the balance plug that feeds the little fan . I used those cables http://www.banggood.com/DIY-1_25mm-2-Pin-Micro-Male-Female-Connector-Plug-Cable-for-RC-LIPO-Battery-FPV-Drone-Quadcopter-p-1080391.html?p=RZ3108607119201405OL
+ i can get goggles battery monitor!


Now the power for the module is independent, 
After that little mod that makes my goggles more “healthier” from damaging the regulator with those power demanding modules, I added into the realacc module a 78m05 5v 0.5amp voltage regulator, 
http://www.alldatasheet.com/datasheet-pdf/pdf/31368/TOSHIBA/78M05.html

<h1>INSTRUCTIONS  FOR THE SOFTWARE </h1>
 Download the https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/releases/download/V2.0/MICRO.MINIM.OSD.SOFTWARE.zip

<h2>Preparation for MicroMinim OSD</h2>
<h3>Fonts</h3>
In order to upload the fonts to Microminim OSD the easiest method is the MW_OSD project.
* connect the microminim osd to pc 
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/MicroMinimOSD-FTDI.jpg?raw=true" width="640"/>
* upload the MW_OSD.ino.hex to Microminim OSD
* open MW_OSD_GUI.exe
* Connect to the MicroMinim
* Font Tools > select the  polyphemous_Charset .mcm
* upload.
* Done with Fonts.

If you are not familiar with this process you can follow this video https://www.youtube.com/watch?v=svIjwDp8T60 , and when your in the part of fonts you choose polyphemous_Charset .mcm from zip file.

<h3>PolyPhemus</h3>
Upload the PolyPhemus.ino.hex into the MicroMinimOSD

<h2>Preparation for RealAcc</h2>
Upload the rx5808-pro-diversityGc9n.ino.hex


<h1>INSTRUCTIONS  FOR THE HARDWARE</h1>
<h2>The Goggles FacePlate mod</h2>
We have to take external power because fatsharks internal voltage regulator not giving at least 0.5amp of current SO.
In my humble opinion everyone that uses diversity module of any brand have to make this little mod.
You are not "hurting" your goggles. Your goggles stays intact .

<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/1.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/2.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/3.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/4.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/5.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/6.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/7.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/8.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/9.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/10.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/11.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/12.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/13.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/14.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/15.JPG?raw=true" width="640"/>
<img src="https://github.com/gc9n/rx5808-Diversity-RealAcc-Compatible/blob/master/STEPS/STEP%20ONE%20(FacePlate)/16.JPG?raw=true" width="640"/>

<h2>Voltage regulator for module</h2>
We scratch this area top peal off the paint carefully (it,s ground) , and we solder the bottom of 78m05

<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/STEP%20TWO%20(Voltage%20regulator%20for%20module)/1.JPG?raw=true" width="640"/>

<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/STEP%20TWO%20(Voltage%20regulator%20for%20module)/2.JPG?raw=true" width="640"/>
 
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/STEP%20TWO%20(Voltage%20regulator%20for%20module)/3.JPG?raw=true" width="640"/>
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/STEP%20TWO%20(Voltage%20regulator%20for%20module)/4.JPG?raw=true" width="640"/>

<h2>VIDEO IN AND OUT</h2>
This is the most important part , this is were you split the video in half and you give it to the OSD and OSD returns the Overlay .

Carefully start scratching this line to peal off the paint
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/10.jpg" width="640"/>

<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/11.jpg" width="640"/>

<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/12.jpg" width="640"/>

now separate this line , cut it in half , and connect to the osd , see pic bellow

<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/13.jpg" width="640"/>

And looks like this 

<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/vinvout.jpg" width="640"/>



 <h2>Cut the VCC pin from the RealAcc Module!!!</h2>
 <h2>And also Cut the VCC pin from the RealAcc Module!!!</h2>
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/pinvcc.jpg" width="640"/>


 <h1>The Connection Diagram </h1>

<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/STEP%20THREE%20(connections)/Realacc%20-%20MinimOSD%20mod%20.jpg" width="1080"/>


 
<h2> Important notice </h2>
You have to consider how your gonna connect the FTDI part of the micro minim osd (RX TX VCC GND) . it have to be disconnected from realacc module easily because if you want to upgrade your firmware in osd or in diversity module they have to be separate. you can see in this pic that i insert Female headers into the osd, in order to take it apart from the module.

<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/1.jpg" width="640"/>

<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/2.jpg" width="640"/>
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/3.jpg" width="640"/>
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/4.jpg" width="640"/>
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/5.jpg" width="640"/>
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/6.jpg" width="640"/>
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/7.jpg" width="640"/>
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/8.jpg" width="640"/>
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/9.jpg" width="640"/>


<h1> To do ! </h1>

After hours-days  of research and development  , try  and error , disappointment ,satisfaction, anger , happiness . 
i came up with this spaghetti! 
now i have to clear up the wires and snag the osd under oled 
<img src="https://raw.githubusercontent.com/gc9n/rx5808-Diversity-RealAcc-Compatible/master/STEPS/PART%20FOUR%20(Connections)/IMG.jpg" width="640"/>



If this project help you reduce time to develop, you can give me a cup of coffee :)

<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=GZKDUKL4C2H5A&lc=GR&item_name=George&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted" target="_blank">
  <img src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" alt="Donate George Chatzisavvidis"  > 
</a> 



V1.0
# rx5808-Diversity-RealAcc-Compatible
RX5808 Diversity RealAcc Compatible

Based on sheaivey/rx5808-pro-diversity project

Added extra features with Favorites tab 

 
 
 <p align="center">
  <img src="https://static.rcgroups.net/forums/attachments/2/6/7/4/6/6/a9522549-129-IMG_0113.JPG" width="640"/>
  <img src="https://static.rcgroups.net/forums/attachments/2/6/7/4/6/6/a9433976-3-IMG_0101.jpg" width="640"/>
</p>

If this project help you reduce time to develop, you can give me a cup of coffee :)

<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=GZKDUKL4C2H5A&lc=GR&item_name=George&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted" target="_blank">
  <img src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" alt="Donate George Chatzisavvidis"  > 
</a> 
