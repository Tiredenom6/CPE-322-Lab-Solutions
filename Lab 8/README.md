## Lab 8 - Data Analysis

## Notes
1) Like in previous labs, the use of sudo is not required in Msys2 and the commands can be preformed without it.

## Steps for Graphing and Data Analysis
1) Run the following commands to install numpy scipy scikit-learn matplotlib pandas tensorflow keras.
            
            $ pip3 install numpy scipy scikit-learn matplotlib pandas tensorflow keras

2) copy the files plt_final.py and plt_cv2.py using teh following commands.
            
            $ cd ~/demo
            
            $ cp ~/iot/lesson8/plt_final.py .
            
            $ cp ~/iot/lesson8/plt_cv2.py .
            
3) edit the files to change the data types to match the excel sheet. 
           
            $ nano plt_final.py  --> data = read_csv('rpidata.csv')
            
            $ nano plt_cv2.py    --> X = read_csv('rpidata.csv', usecols=[1])
            
                                 --> Y = read_csv('rpidata.csv', usecols=[2])
4) Run the scripts as follows,

            $ python3 plt_final.py
            
            $ python3 plt_cv2.py


## Results
1) The results is an output of a series of graphs. These graphs can be seen in the images folder of this Lab.

