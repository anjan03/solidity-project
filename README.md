# Introduction
This was the final project of the solidity beginner course of the metacrafters. Here we created how to mint and burn tokens using the solidity programming language . 
we used the remix IDE for this project from the ethereum community. (https://remix.ethereum.org/). 

# Description 
In this project we used the solidity programming language we used 2 function's to mint and burn the tokens . This program serves as a simple and straightforward introduction to Solidity programming, and can be used as a stepping stone for more complex projects in the future.

# Getting started
You can copy paste the above given program in the remix editor which is freely available online (https://remix.ethereum.org/).
The following are the mint and burn functions that we have written in the project and both the functions take 2 parameters(address and value) respectively.
```
function mint (address _address,uint _value) public{
        totalSupply += _value;
        balances[_address] += _value;

    }
    // burn function
    function burn (address _address,uint _value) public{
        if (balances[_address] >= _value){
            totalSupply -= _value;
            balances[_address] -= _value;
        }
    }
```
# License
This project is licensed under the MIT License - see the LICENSE.md file for details
