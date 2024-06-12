# Introduction:

It is simple smart contract ( MY TOKEN ) for minting and burning tokens on the Ethereum blockchain.

# Description:

MyToken is a simple Solidity-implemented token contract that resembles an ERC20. It enables the tracking of the total supply and balances of individual addresses, as well as the minting of new tokens and the burning of old ones. The purpose of this contract is to serve as a teaching tool for fundamental token management and smart contract creation.

# Characteristics:

- Accessible variables to store information about tokens, such as name, symbol , and quantity available.

- Mapping for tracking the token balance of each address.

- A function with the required validations for creating new tokens and removing existing ones.


# Contract Details:


## - *Variables Used*

*tokenName(string):* Data type used string for given a name to the token.(Token Name: Simple)

*tokenSymbol(string):* This  gives a shortform for the token.(Token Symbol: Dot)

*totalSupply(uint):* Data type used uint i.e only positive number, this gives the amount of token .(Initialised:30)

## - *Mapping*

*balances:* An association between addresses and token balances.


## - *Functions*
  
*mint(address _ads, uint _value):* This function adds the designated amount to the address's balance and raises the total token supply.

*burn(address_ads, uint_value):*This function subtracts the specified amount from the address's balance and reduces the total token supply. Before continuing, it makes sure that the address's balance is more than or equal to the burnt.

# *Usage*


- *Deployment:* We must select the "Deploy" option in order to initiate the contract.  
- *Minting Token:* Use the mint function and enter the address and desired number of tokens to be minted in order to create new ones. For example, you can use mint(0xAbc123..., 100) to add 100 tokens to the address 0xAbc123...
- *Burning token:* Use the burn function and enter the address and quantity of tokens to be burned in order to eliminate them. For example, you can use burn(0xAbc123....., 50) to extract 50 tokens from the address 0xAbc123....., but only if there is sufficient balance.
