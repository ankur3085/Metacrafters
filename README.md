# Metacrafters Beginner Module 
This Solidity smart contract implements a basic token called "Gol Gappa" (GG). The contract allows for token minting and burning, while keeping track of token balances for different addresses.
## Getting Started
- Remix
## Usage

##### Mint Function
```
// Mint function to create new tokens
    function mint(address _address, uint _value) public {
        totalSupply += _value;
        balances[_address] += _value;
    }
```
##### Burn Function
```
function burn(address _address, uint _value) public {
    if(balances[_address]>= _value)
        totalSupply -= _value;
        balances[_address] -= _value;
    }
```
## Authors
- Ankur Pandey
