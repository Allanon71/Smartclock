# SMARTCLOCK

> Author  : Fabio Falcucci (Allanon)  
> Contact : info@a-mc.biz  
> License : Freeware  

If you like my work and you want to buy me a coffee you can support me on Patreon https://www.patreon.com/Allanon71  or with PayPal to mailto:hijoe@tin.it   
:D

## INTRODUCTION
I've made this program for my personal use so it's not a full fledged application but some things has been hacked like the RSS Reader that just looks for specific strings headers instead of parsing the XML file.

I've provided a **config.txt** where you can configure the clock has you like, you can also completely change the layout since elements can be positioned and scaled as you wish.
The 7 segment display and the dot matrix display are implemented in the provided **DigitalWorld.hws** include.

## BEFORE YOU RUN
Before you run the program you need my libraries that you can find here : https://github.com/Allanon71/Hollywood-MAL-Libraries
Download them and configure them as explained below:
My libraries use a global include file called **+Includes.hws** where all library names are defined along with their path, in order to run the program you need to setup the variable **#INC_PATH** with the absolute path where you have saved/cloned the libraries, if you do this you will be able to run all the examples with a double click, for example let's suppose you have cloned the entire repository into the following path : `C:/MyHollywoodStuff/Libs/`  
All you have to do is:  
+ Open the file `+Includes.hws`  
+ Edit the line `Const #INC_PATH     = ""`  
+ Putting the absolute location, in our case `C:/MyHollywoodStuff/Libs/`  
+ Save the edited file  

After this step open the **includes.hws** file in the SmartClock folder and specify the full path of the **+Includes.hws** file in the line:
```plaintext
@INCLUDE "=== PUT HERE THE PATH TO +Includes.hws FILE ==="
```

The last step is to obtain the OpenWeather API Key, it's free and you can request it in a couple of clicks here : https://openweathermap.org

Replace your own key with the one provided because free accounts have a limited daily number of requests available, but enough for this project :)  

Now you are ready!


---

## ABOUT SMARTCLOCK
This is a clock app developed to run on my Raspberry Pi4, it features a digital clock emulating 7 segments display and 2 dot matrix display (fully configurable) to display the current wheater and forecast and the latest news taken from an RSS Feed.

The clock features a Dim mode to change the color in certain times (for example to use softer colors during the night), it also has a screensaver that run an animation on the 7 segments display to avoid static images for too long.

 ---
 Latest update: 19/12/2020
 ---