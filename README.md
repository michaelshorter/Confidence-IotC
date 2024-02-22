# Confidence-IotC
Code exploring the mechanics of speech to text technologies. This device listens to everything it can hear and tells users how confident it was in what it heard, both in terms of individual words but also constructed sentences. This allows users to see not just the confidence levels of speech recognition but also see the words that it didn't hear that it uses machine learning to assume.  

## Setup
### First we need to turn it on and connect to wifi:
1. First use a USB-C cable to power up the device. This is done by pushing it through the hole at the back.
2. We then need to connect a mouse and keyboard via the usb socket on the side. Ideally we use a wireless mouse and keyboard that work from the same dongle other wise you will need to keep swapping between the mouse and the keyboard as there is only one USB socket.
3. Once the device has loaded up and you  an see the desktop on the screen make sure it is connected to the wifi by clicking on the wifi logo at the top right hand side of the screen. If it is not connected find a network and connect.


### Now it is time to run the code:
1. open a new terminal window (control+alt+t)
2. Make full screen (fn+F11) (or right click and select full screen).
3. type the following
   ```
   cd WordCloud/AzureSpeechCC
   ```
4. Press return
5. Type the following
   ```
   dotnet run
   ```
11. The code should now be running. It should now say "Ready Speak"


### Now we can connect the Microphone:
1. Make sure the code is in full screen.
2. Make sure the mouse is not visible on the screen by moving it to one side
3. Un-plug the mouse/keyboard
4. Plug in the microphone

   
### To shutdown safely:
1. To exit program hit press Control+z
2. Unplug the microphone
3. Plug in the mouse
4. NAvigate to the top right menu, click to select shutdown.
   


## If making changes:
```
dotnet clean
dotnet build
dotnet run
```




## TO SETUP THE 3.5 INCH RPI SCREEN:

Here: https://github.com/lcdwiki/LCD-show-ubuntu

sudo rm -rf LCD-show-ubuntu

git clone https://github.com/lcdwiki/LCD-show-ubuntu.git

chmod -R 755 LCD-show-ubuntu

cd LCD-show-ubuntu/

sudo ./LCD35-show


To revert back to monitor:
sudo ./LCD-hdmi
