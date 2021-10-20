# CryptoZombies
Learning solidity on cryptozombies.io

1) Contracts are the building blocks of ethereum applications.


2) The first line of Solidity code should sepcify the compiler version it needs. the synatx is: pragma solidity //version range.


3) State variables are variables stored to the memory of the contract. These values are written to the blockchain. 
        
          uint means unsigned integer. 
          uint is 256 bits by default.
          uint can also be uint8, uint16, uint32.
          
          
4) Modulus (%) operator returns the remainder of a division between two numbers.
          13 % 5 = 3.
          
   Exponential operator ( ** ) adds power to the number.
          5 ** 2 = 5 to the power of 2 = 25
          
          
5) A struct is a way to store complex data types, which combine more than one value-type. 

          Syntax: struct //name// {
          
            uint //name//;
            string //name//;
            
           }
           
           
6) Solidity has two types of arrays: fixed arrays and dynamic arrays.

>>      Fixed arrays have a specified length.

          Syntax: uint[2] fixedArray;
          
        
>>      Dynamic arrays have a dynamix length.
        
           Syntax: uint[] dynamicArray;
           
           
>>       An array of structs can be be created by 
  
