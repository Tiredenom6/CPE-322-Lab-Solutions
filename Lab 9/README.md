## Lab 9 - Yang

## Steps for PlantUML to Intrusiondetection.png
1) Run the following commands to install pyang and plantuml

          $ sudo pip3 install pyang plantuml
            
2) run the following commands to make the output to make an image by converting between yang yin and uml file extensions.
          
          $ sudo pip3 install pyang plantuml
          
          $ mkdir ~/demo
          
          $ cp ~/iot/lesson9/intrusiondetection.yang ~/demo
          
          $ cd ~/demo
          
          $ cat intrusiondetection.yang
          
          $ pyang -f yin -o intrusiondetection.yin intrusiondetection.yang
          
          $ cat intrusiondetection.yin
          
          $ pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef
          
          $ cat intrusiondetection.uml
          
          $ python3 -m plantuml intrusiondetection.uml
          
## Results
The result of this code is the creation of a png file called intrusiondetection.png which is available for viewing in the folder.  
