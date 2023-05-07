## Lab 7 - Thingspeak and GoogleSheets

## Notes
1) Like in previosu labs, the use of sudo is not required in Msys2 and the commands can be preformed without it.
2) There are common issues with installing psutil

        1) Install Wheel
        2) To chekc to see why it fails use $ python -m pip show requests and download the missing packages.
        3) use cygwin to download the missing package
        4) pacman -S mingw-w64-x86_64-python-psutil to download if using msys2. 
        5) Uninstall python and pip and reinstall to avoid msys error. It is not supported for Msys or MINGWIN

## Steps for ThingSpeak Demonstration
1) Run the following commands to install psutil and to connect your computer to Thingspeak
            $ sudo pip3 install -U psutil
            
            $ cd ~/demo
            
            $ cp ~/iot/lesson7/thingspeak_cpu_loop.py .
            
            $ cp ~/iot/lesson7/thingspeak_feed.py .
            
            $ cat thingspeak_cpu_loop.py
            
            $ cat thingspeak_feed.py
            
            $ python3 thingspeak_feed.py

2) Check your output on thing speaks. Mine can be found in the Thingspeak feed.png image in this folder. 

## Results
1) The Result was that the terminal would update when it sent messages to Thingspeak and showed the data graphed on the Mathworks website. 

## Steps for Google Cloud Platform

1) Download and install gspread using the following command
 
        $ pip3 install -U gspread oauth2client
        
2) Create a cloud based excel api using google sheets     
          
3) Download your .json file and use the cat command in terminal to edit the file rpi_spreadsheet.py

5) Run your program using the command 

        $ python rpi_spreadsheet.py
## Results         
This will output both the cpu usage and memory available to an excel sheet. This can be seen in the images folder under cloud based excel.png. 


