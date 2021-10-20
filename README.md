# CryptoZombies
Learning solidity on cryptozombies.io

1) Contracts are the building blocks of ethereum applications.


2) The first line of Solidity code should sepcify the compiler version it needs.                         

          Synatx: pragma solidity //version range//

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

      Fixed arrays have a specified length.

          Syntax: uint[2] fixedArray;
          
        
      Dynamic arrays have a dynamix length.
        
           Syntax: uint[] dynamicArray;
           
           
An array of structs can be be created by replacing the variable-type with the struct name

           Syntax: //struct name//[] arrayName;
           
           
'Public' arrays are arrays which are visible to other contracts. Solidity generates a 'getter' method for these arrays. 

           Syntax: structName[] public arrayName;
           
           

7) Functions have the following syntax:

           function funcName(string memory _name, uint _amount) public {
           
           }
           
'string' and 'uint' are the parameters that the function takes. This means, when the function is called it will also be assigned a string value and a uint value, that the function will process. This is how a function is called:

           funcName("PM", 25);
           

Pass by value vs Pass by reference

          In reference to uint x = 42, 'passed by value' means that when x is called
          to a function and 'passed', the function picks up the value stored in x,
          without impacting x itself.
          

  
