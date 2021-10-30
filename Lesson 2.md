Lesson 2

1) Mappings are primitive that allow you to store a key-value combination. The mapping has a declared key type and a value type; then a declaration as to whether it is a public mapping or not; and then the name of the mapping.

        Syntax: mapping (//key-type// => //value-type//) //nameOfMapping//;
        Example: mapping (int => string) rollNumToName;
    

2) msg.sender 

This is a 'universal variable available to all functions' in Solidity. Essentially, it represents the address of the contract that calls the function 
