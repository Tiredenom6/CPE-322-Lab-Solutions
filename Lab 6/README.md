## Lab 6 - Node.js and Pystache. 


## Lab Requirnments
This lab requires you to download Node.js at the following link " https://nodejs.org/en/download" 
## Notes
1) Like in previosu labs, the use of sudo is not required in Msys2 and the commands can be preformed without it.
## Steps for Node.js
1) Run the following commands
            $ node -v
            
            $ npm -v  
            
            $ node -h
            
            $ cd ~/iot/lesson6
2) Run the following command 
            $ node hello-world.js
            
This will output Hello world to the address http://127.0.0.1:3000/ in a web page

3) Run the next command 
            $ node hello.js

This will output Hello world! to the address http://127.0.0.1:8080/ in a web page. However this will return in standard output a message everytime the page is accessed. 
            
## Results
1) The result of the first command was a web page that viewed hello world and can be viewed in the image Hello world.png.  
2) The result of the second command was the same web page but with a return every time it was accessed in the terminal. This can be seen in the Hello World2.png image. 

## Steps for Pystache

1) Download and install Pystache using the following command
 
        $ pip3 install pystache
        
2) Enter the repository with the following command     
        
        $ cd ~/iot/lesson6
        
3) Preform the following two commands to run say_hello.py in the template of say_hello.mustache
        
        $ cat say_hello.mustache
        
        $ cat say_hello.py

4) Run say_hello.py
        
        $ python3 say_hello.py
## Results         
This output say_hello.py onto the terminal and output text. The text can be seen in the image in this file named Hello Alex.png
