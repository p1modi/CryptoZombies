Lesson 2

1) Mappings are primitive that allow you to store a key-value combination. 

Step 1: Declare the mapping. The mapping has a declared key type and a value type; then a declaration as to whether it is a public mapping or not; and then the name of the mapping.

        Syntax: mapping (//key-type// => //value-type//) //nameOfMapping//;
        Example: mapping (int => string) rollNumToName;

Step 2: Assign value to the mapping by using [] for the key and = for the value.

        Syntax: rollNumToName[25] = "Pranay Modi";

2) msg.sender 

This is a 'universal variable available to all functions' in Solidity. Essentially, it represents the address of the contract that calls the function where the msg.sender variable is located.

          Syntax: [use msg.sender in place of variables].

          Example of using mappings with msg.sender:
          
         mapping (string => address) nameToAddress;
         nameToAddress["Pranay"] = msg.sender;
         
