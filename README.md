# __CricketFanToken (CFT) Contract__

CricketFanToken is an ERC20 token contract implemented in Solidity. It utilizes OpenZeppelin's ERC20 and Ownable contracts to provide standard token functionality and ownership control.
# Description

CricketFanToken (CFT) is an ERC20 token contract deployed on Ethereum. It provides essential token operations such as transfer, approve, and transferFrom. Additionally, it includes features for minting tokens by the contract owner and burning tokens by holders. This contract is designed to cater to cricket enthusiasts and fans within decentralized applications and platforms.

This description gives a brief overview of your project as well as a summary of what the contract code implements. It's aimed at providing a clear and concise introduction to potential users and developers interested in your CricketFanToken contract. Adjust it further based on any additional unique features or specific aspects of your project you wish to highlight.








## Getting Started
### Installing
To download the code, you can visit the following file path:-[https://github.com/Sagarthakur18/ETH-AVAX_assesment_3/blob/main/assesment3.sol]

## Executing program
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at (https://remix.ethereum.org/.)

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., Meta.sol). Copy and paste the following code into the file: contract MyToken
```

      constructor() ERC20("CricketFanToken", "CFT") Ownable(msg.sender) {
        // Mint initial supply to the contract deployer (owner)
        _mint(msg.sender, 1000000 * 10 ** decimals());
    }

    function mint(address to, uint256 amount) public onlyOwner {
        _mint(to, amount);
    }

    function burn(uint256 amount) public {
        _burn(msg.sender, amount);
    }

    // Function to retrieve the balance of an address
    function balance(address account) public view returns (uint256) {
        return balanceOf(account);
    }
}
  

   

 

   
```
## Authors
Sagar Thakur (sagarthakur8456@gmail.com)

## License
This project is licensed under the MIT License - see the LICENSE.md file for details
