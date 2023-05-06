## Lab Three - Python


This lab has a few requirnments in order to complete it.

      1) You must install Python which can be found here " https://www.python.org/downloads/ "
            i) Be sure to include Python in path when installing
            
      2) Then you must install pip which can be done using the command $ py -3.11 --version
      
      3) Next instal jdcal, astral and geopy using the following commands,
                    1) pip install jdcal
                    2) pip install astral
                    3) pip install geopy
 ## Notes
 If an error occurs when making this lab, try using these two commands in the Msys2 terminal 
 
          1) $ pacman -S python3
          2) $ pacman -S python3-pip
          
 ## Steps and Output of each step
1)      $ cd ~/iot

2)      $ cd *3

3)      $ python3 julian.py
        Output:
        Calendar Date: 2023-05-06
        Julian Date: 2460070.5
        Modified Julian Date: 60070.0

4)      $ python3 date_example.py
        Output:
        Date: 2023-05-06
        Date: 05-06-23
        Day of Week: Saturday
        Month: May
        Year: 2023
        103 days after the first day of classes
        3 days before the last day of classes
        
5)      $ python3 datetime_example.py
        Output:
        2023-05-06 18:07:21.649624
        2023-05-06 18:07:21.649686
        2023-05-06 22:07:21.649701
        1683410841.6501157
        Sat May  6 18:07:21 2023
        2023-05-06 18:07:21.650158
        2023-05-06 22:07:21.650181

6)      $ python3 time_example.py
        Output:
        Sat May  1 18:08:12 2023
        
8)      $ python3 moon.py
        Output:
        2023-05-06 Moon Phase: 14
        2023-05-07 Moon Phase: 15
        2023-05-08 Moon Phase: 16
        2023-05-09 Moon Phase: 17
        2023-05-10 Moon Phase: 18
        2023-05-11 Moon Phase: 19
        2023-05-12 Moon Phase: 20
        2023-05-13 Moon Phase: 21
        2023-05-14 Moon Phase: 22
        2023-05-15 Moon Phase: 23
        2023-05-16 Moon Phase: 24
        2023-05-17 Moon Phase: 25
        2023-05-18 Moon Phase: 26
        2023-05-19 Moon Phase: 27
        2023-05-20 Moon Phase: 0
        2023-05-21 Moon Phase: 1
        2023-05-22 Moon Phase: 2
        2023-05-23 Moon Phase: 3
        2023-05-24 Moon Phase: 4
        2023-05-25 Moon Phase: 5
        2023-05-26 Moon Phase: 6
        2023-05-27 Moon Phase: 6
        2023-05-28 Moon Phase: 7
        2023-05-29 Moon Phase: 8
        2023-05-30 Moon Phase: 9
        2023-05-31 Moon Phase: 10
        2023-06-01 Moon Phase: 11
        2023-06-02 Moon Phase: 12
        2023-06-03 Moon Phase: 13
        2023-06-04 Moon Phase: 14
        
9)      $ python3 coordinates.py 'SC Williams Library'
        Output:
        Library Parking, Williams Lake, Cariboo Regional District, British Columbia, Canada
        (52.130143399999994, -122.14187089155848)

10)     $ python3 address.py '40.74480675, -74.02532862031404'
        Output:
        Samuel C. Williams Library, Field House Road, Hoboken, Hudson County, New Jersey, 07030, United States
        (40.74480675, -74.02532861159351)
        
11)     $ python3 cpu.py
        Output:
        
        
12)     $ python3 battery.py

13)     $ python3 documentstats.py document.txt
         Output: 
         Word Count: 1343
         Top Ten Words: [('our', 26), ('their', 20), ('has', 20), ('he', 19), ('them', 15), ('these', 13), ('have', 11), ('we', 11), ('us', 11), ('people', 10)]
