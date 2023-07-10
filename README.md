# Metacrafters--EVM-Proof-Beginner
This is a simple ERC-20 token contract implemented in Solidity. The contract allows for the creation and destruction of tokens, as well as storing information about the token.

# Requirements
1. The public variables in the contract include the information about the coin:
tokenName: A string that represents the token's name.
abbrv: A string that represents the token's abbreviation.
totalSupply: An unsigned integer that represents the token's entire supply.
2. The contract has an address to balance mapping:
balances: An association between addresses and the accompanying token balances.
3. The contract provides a mint function that adds a specified amount to both the balance at the "sender" address and the overall supply:
   
Parameters:
_address: The address to which the tokens will be minted.
_value: The amount of tokens to be minted.
Actions:
~ Increase the totalSupply by _value.
~ Increase the balance of the _address by _value.

5. The contract has a burn function that decreases the total supply and the balance of the "sender" address by a given value:

Parameters:
_address: The address from which the tokens will be burned.
_value: The amount of tokens to be burned.
Actions:
Check if the balance of the _address is greater than or equal to _value.
If true, decrease the totalSupply by _value.
Decrease the balance of the _address by _value.
# Usage
Install the MyToken contract on an Ethereum network that is supported.
When the contract is launched, you may communicate with it by calling the following functions:
mint: allocates newly created tokens to a certain address.

Parameters:
_address: The address to which the tokens will be minted.
_value: The amount of tokens to be minted.
burn: Reduces the total supply and the balance of a given address by burning existing tokens.

Parameters:
_address: The address from which the tokens will be burned.
_value: The amount of tokens to be burned.
# License
The MIT License governs this agreement. MIT is the SPDX-License-Identifier.
