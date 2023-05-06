### The lab consisted of creating a directory file and loading coded programs into it. Following this I ran the code through Msys2.

### Notes: 
  1) If using Msys2 terminal, you must change the application properties target to include usage of the full path.
          1) open Msys terminal
          2) Go to the file location and right click
          3) click view properties 
          4) change the target to " C:\msys64\msys2_shell.cmd -msys -use-full-path  " 
          5) (do not include the parentheses) 
 
 2) To change the file path, go to environment variables - advanced and then click on path under system variables. 
 3) Add the Downloaded files to your path. 
 4) you can copy the cloned repository form the lab into your Msys home file location manually if you have trouble with the following command 
                                     cp ~/dsd/ghdl/*vhdl .
                                     
                                  
 ### To run the dff.vhdl or D flip flop file use the following commands in terminal 
```sh
$ ghdl -a tff.vhdl
$ ghdl -a tff_tb.vhdl
$ ghdl -e tff_tb
$ ghdl -r tff_tb --vcd=tff.vcd
$ gtkwave tff.vcd
```

### To run the adder.vhdl or the Full adder use the following commands in terminal 
```sh
$ ghdl -a adder.vhdl
$ ghdl -a adder_tb.vhdl
$ ghdl -e adder_tb
$ ghdl -r adder_tb --vcd=adder.vcd
adder_tb.vhdl:54:5:@8ns(assertion note): end of test
$ gtkwave adder.vcd
```

### To run the ha.vhdl or the half adder use the following commands in terminal  
```sh
$ ghdl -a ha.vhdl
$ ghdl -a ha_tb.vhdl
$ ghdl -e ha_tb
$ ghdl -r ha_tb --vcd=ha.vcd
ha_tb.vhdl:47:5:@5ns:(assertion error): Reached end of test
$ gtkwave ha.vcd
```

                                  
                    To see the products of the assignemnt, please see the PNG files, Photos will not regsiter with commands. ERROR 282
                                  


          
          
   
