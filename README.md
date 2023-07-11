# Sweet-Home
This is a simple token contract that is built using Solidity.

I have created the following variables for MyToken:

- tokenName: a public string variable representing the name of the token(Sweet).
- tokenAbbry: a public string variable representing the abbreviation of the token(Home).
- totalSupply: a public uint variable representing the total supply of the token.

The term "mapping" is used to construct a data structure that converts one type of data to another. The "balances" variable in this code is a mapping that maps addresses to their associated token balances. The mapping uses the "address" type as the key and the "uint" type as the value.

I have created the following Functions:

- mint: a public function that adds to the total supply and increases the balance of a specified address.
- burn: a public function that subtracts from the total supply and decreases the balance of a specified address, only if the balance is greater than the value being burned.

Conditional statement:
The "if" statement is a conditional statement that executes a block of code only if a certain condition is true. In this code, the "burn" function includes an "if" statement that checks if the balance of the specified address is greater than or equal to the value being burned. If the condition is true, the code inside the "if" block will be executed, which subtracts the value from the total supply and from the balance of the specified address.

The ">= operator" checks if the balance is greater than or equal to the value being burned. If the balance is equal to the value being burned, the balance will become zero after the "burn" function is called. If the balance is less than the value being burned, the "if" block will not be executed, and the balance and total supply will remain unchanged.
