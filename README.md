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
           
           
6 & 8) Solidity has two types of arrays: fixed arrays and dynamic arrays.

      Fixed arrays have a specified length.

          Syntax: uint[2] fixedArray;
          
        
      Dynamic arrays have a dynamix length.
        
           Syntax: uint[] dynamicArray;
           
           
An array of structs can be be created by replacing the variable-type with the struct name

           Syntax: //struct name//[] arrayName;
           
           
'Public' arrays are arrays which are visible to other contracts. Solidity generates a 'getter' method for these arrays. 

           Syntax: structName[] public arrayName;
           

An entry can be added to the end of an array by using the following command:

          arrayName.push(//contents that go into the array//);
          
Example of an array of structs, with the push command:

          struct phone {
                    string phoneName;
                    uint modelNumber;
                    }
                    
          phone[] public arrayOfPhones;
          
          phone ABC = phone("iPhone", 8);
          
          arrayOfPhones.push(ABC);
          
          OR
          
          arrayOfPhones.push(phone("iPhone", 8);


7) Functions have the following syntax:

           function funcName(string memory _name, uint _amount) public {
           
           }
           
'string' and 'uint' are the parameters that the function takes. This means, when the function is called it will also be assigned a string value and a uint value, that the function will process. This is how a function is called:

           funcName("PM", 25);
           
Function parameters are conventionally named using an underscore that precedes the name ('_ name'). This is to distinguish them as variables that operate within the function. Global variables - whcih operate in the entire contract - do not get underscores before them.


'memory' indicates that the '_ name' variable should be sotred in memory as opposed to storage. All reference types are required to be stored in memory, and require the 'memory' syntax to be used.

When a fucntion iterates on a data-type, it is known as 'passing' that data-type.

Based on the data-type in consideration, the function either passes 'by value' or 'by reference'.

Pass by value vs Pass by reference

          In reference to uint x = 42, 'passed by value' means that when x is called
          to a function and 'passed', the function picks up the value stored in x,
          without impacting x itself.
          
          In reference to uint[] x = [0,1]; 'passed by reference' means that when x
          is called to a function and 'passed', the function iterates by making a
          reference to the array x and the iterations impact that array.
          
Some data-types are Value Types (always passed by value) while others are Reference Types (always passed by reference).

          Value Types: booleans, integers, fixed point numbers, address,
          contract types, fixed-size byte arrays, dynamically-sized byte arrays,
          Address Literals, Rational and Integer Literals, String Literals and
          Types, Unicode Literals, Hexadecimal Literals, Enums, Function Types
          
          
          Reference Types: Data location, arrays, array slices, structs.

  
9) Functions can be public or private. 
          
          Public functions can be called by anyone or any other contract. 
          This means that any other contract will be able to execute the code in
          that public function. 
          
          Private functoins can only be called by other functions within the
          same contract. 

It is also conventional to name private functions by using an underscore before their name.


10) 
