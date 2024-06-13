# Solidity_beginner
---

# HemanthToken

## Introduction

HemanthToken is an ERC20-like token implemented in Solidity. This smart contract allows for minting and burning tokens, with public variables to store details about the token and a mapping to keep track of balances.

## Contract Details

### Public Variables

- `TokenName`: The name of the token. 
- `TokenAbb`: The abbreviation of the token.
- `TotalSupply`: The total supply of tokens in existence.

### Mapping

- `balances`: A mapping from addresses to their corresponding token balances.

### Functions

#### `mint`

The `mint` function allows for the creation of new tokens. It takes two parameters: an address and a value. The function increases the total supply by the specified value and increases the balance of the specified address by that amount.

```solidity
function mint(address _address1, uint _value1) public
```

#### `burn`

The `burn` function allows for the destruction of tokens. It takes two parameters: an address and a value. The function decreases the total supply by the specified value and decreases the balance of the specified address by that amount. The function includes a check to ensure that the balance of the specified address is greater than or equal to the amount to be burned.

```solidity
function burn(address _address1, uint _value1) public
```

## Usage

1. **Deploy the Contract**: Deploy the HemanthToken contract to the Ethereum network.

2. **Mint Tokens**: Use the `mint` function to create new tokens. Provide the address and the amount of tokens to mint.

3. **Burn Tokens**: Use the `burn` function to destroy tokens. Provide the address and the amount of tokens to burn. Ensure the address has enough balance to burn the specified amount.

## License

This project is licensed under the MIT License.

---
