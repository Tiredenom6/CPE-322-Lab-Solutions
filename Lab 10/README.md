## Lab 10 - Blockchain

## Steps for Comparing Hash values 
1) Run the following two commands and compare the output.

          $ cd ~/iot/lesson10
          
          $ python hash_value.py
            
The following two outputs are as follows, 

      Output 1
      
          The hash for 1 is: 1
          
          The hash for 1.0 is: 1
          
          The hash for 3.14 is: 322818021289917443
          
          The hash for Python is: 9012037900203850788
          
          The hash for a tuple of vowels is: 1656869808690947643
          
          The hash for an object of person is: 7909072654561468049


      Output 2

          The hash for 1 is: 1
          
          The hash for 1.0 is: 1
          
          The hash for 3.14 is: 322818021289917443
          
          The hash for Python is: 6711810364895373297
          
          The hash for a tuple of vowels is: -6921545617625019888
          
          The hash for an object of person is: 5026911483776632655
          
## Steps for running snakecoin.py
1) Direct to the file 

          $ cd ~/iot/lesson10
          
2) If you would like to view the file use the following command
          
          $ cat snakecoin.py
         
3) Run the code using the following  
        
          $ python3 snakecoin.py

The output is as follows,

Block #1 has been added to the blockchain!
Hash: 3933e71fdb1e772c50d146a822803eb3e829d92ffcd381903cfafde69c197161

Block #2 has been added to the blockchain!
Hash: 95b94442cf268be87aa3bdb52d9c9f5580f83e4fce31886e80c61e142a1b17f3

Block #3 has been added to the blockchain!
Hash: 4293b36aee8adc538ae97598e210c67a0477e0c3d6e12daf65ce418d91fac65c

Block #4 has been added to the blockchain!
Hash: 8b98e4fded362c4ebbfe585ea8897581ba7671a1df885357cc1fa942ba819002

Block #5 has been added to the blockchain!
Hash: 766efd2167bb49ccdaa5d5ea12d58b5f003157cde939f1c8dd5889b0f31ca091

Block #6 has been added to the blockchain!
Hash: 14938cafc77e1990dccc7d2ca58b811d3883268f634ee00f5de4e56a431f762a

Block #7 has been added to the blockchain!
Hash: 861c4cdf88277d300b75fe351442a9edd5e8e120b514fa4d7fd0372f2928d23e

Block #8 has been added to the blockchain!
Hash: fc4191f8efdba9fdfa8bf02df3ab114beb131263533f82d8c368fc11faae5c2e

Block #9 has been added to the blockchain!
Hash: ed1f7b26afb1fee8923825721ea7b12e48a702bed6ffea1d96b8a91553dc8f5f

Block #10 has been added to the blockchain!
Hash: 9a6dba5dac448904f0e7ecf13b9900a801c792fc5719b8585b27ad9d37490e39

Block #11 has been added to the blockchain!
Hash: 72f2919e20b736f431667d384c5384e25914a7ee5abfb1d7b3cb0aaec51d885d

Block #12 has been added to the blockchain!
Hash: afa3ae81fe40ccc1429a6bbf57df60b8ef42cf768468921c2ac1cdcae76466f7

Block #13 has been added to the blockchain!
Hash: e7914bf654fb00947836d63c44945b206120868034e4a9a7ba121e7a4556aed8

Block #14 has been added to the blockchain!
Hash: fe3598214e1686c1e9efed0a5d392acfd3575ebcb66b7f103d1d65255201df98

Block #15 has been added to the blockchain!
Hash: 445fce2fc5e9634eb9ae0486d60ac3a20a61c687e82046b551554a958d1729c6

Block #16 has been added to the blockchain!
Hash: 28c278f2c3d297c43b19888ed1b6997c0b5ea25b367a14136b034c8c4ad7416c

Block #17 has been added to the blockchain!
Hash: d26b7eb2cf548894b38f208c507ef6bf1f4ba794a4287439201eb194a3f3ce8c

Block #18 has been added to the blockchain!
Hash: 07dc4026a91b5bd49249de09eb7519ae31421c57d1bcb8d1e795ea2945d4febb

Block #19 has been added to the blockchain!
Hash: bc14bd8f13be3de69300ea3678aba55ecf793deb190600aba3c3e6be6e6be9d4

Block #20 has been added to the blockchain!
Hash: baaa03ef5726f67022f24df7f7e24701fd5893fe5d46bbd037694722e7f521e1

## Steps for running Snakecoin-server-full-code.py
1) Open a second terminal so that two are open, both are necessary.

2) On Terminal one run the following commands

                    $ cat snakecoin-server-full-code.py
                    
                    $ python3 snakecoin-server-full-code.py
                    
                    $ cd  

3) On Terminal two run the following commands

                    $ curl "localhost:5000/txion" \-H "Content-Type: application/json" \ -d '{"from": "akjflw", "to":"fjlakdj", "amount": 3}'
                    
                    $ curl localhost:5000/mine

4) Visit the web address http://127.0.0.1:5000/ to view your program
 
The results of this can be found in the folder above named Snake Server.PNG as well as the terminal output Snake Server Terminal.PNG. 

## Steps for changing the code
1) Again open up two terminals. 

2) On the first terminal uncomment the last line of node_server.py with the commands bellow,

                    $ git clone https://github.com/satwikkansal/python_blockchain_app.git
                    
                    $ cd ~/python_blockchain_app
                    
                    $ nano node_server.py
                    
                    $ python3 node_server.py

3) On the second terminal run the following code,

                    $ vncserver
                    
                    $ cd ~/python_blockchain_app
                    
                    $ python3 run_app.py
                    
4) Then visit the address http://127.0.0.1:5000 to view results

## Results
The results of this is a website that can be seen in the Yournet.png image and the mined blockchains in the Mined.png in this folder. 
The Yournet created shows who made a blockchain and the mined shows the most recent blockchain mined. 


