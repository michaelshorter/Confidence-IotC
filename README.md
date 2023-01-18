# Confidence-IotC
Code exploring the mechanics of speech to text technologies


To load:
1. open a new terminal window (control+alt+t)
2. cd WordCloud/AzureSpeechCC
3. dotnet run
4. To exit program hit Control+z


If making changes:
dotnet clean
dotnet build
dotnet run


TO SETUP THE 3.5 INCH RPI SCREEN:

Here: https://github.com/lcdwiki/LCD-show-ubuntu

sudo rm -rf LCD-show-ubuntu

git clone https://github.com/lcdwiki/LCD-show-ubuntu.git

chmod -R 755 LCD-show-ubuntu

cd LCD-show-ubuntu/

sudo ./LCD35-show


To revert back to monitor:
sudo ./LCD-hdmi
