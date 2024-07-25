# Swisstronik Testnet Task: Deploy a simple contract using Hardhat
https://www.swisstronik.com/testnet2/dashboard#

## 1) Download and create a swisstronik wallet and get faucet in the task dashboard
https://chromewebstore.google.com/detail/swisstronik/acfhdnikkbldnocbgmfginnmhjfkimjo?utm_team=devs_front&utm_channel&utm_lang=en&utm_date=45216

## 2) Setup Instructions

1. **Clone the Repository:**

    ```sh
    git clone https://github.com/dante4rt/swisstronik-testnet.git
    cd swisstronik-testnet
    ```

2. **Run the Setup Script:**

    ```sh
    ./swisstronik.sh
    ```

3. **Follow the Prompts:**

    - Enter your Swisstronik private key
    - Use the default directory (just press Enter).
    - Press **y** to confirm any prompts.
  
4. **Copy your Contract address**

![Screenshot_122](https://github.com/user-attachments/assets/146f84cb-c210-42bf-9066-2779e4d5e145)


5. **Upload your .sol contract file**

- Create a repository in github
- Create a new file and name it: `Hello_swtr.sol`
- paste following code in it and save it
```sh
// SPDX-License-Identifier: UNLICENSED
pragma solidity ^0.8.19;

contract Swisstronik {
    string private message;

    constructor(string memory _message) payable {
        message = _message;
    }

    function setMessage(string memory _message) public {
        message = _message;
    }

    function getMessage() public view returns(string memory) {
        return message;
    }
```
## 3) Complete task: Deploy a simple contract using Hardhat
**Submit your `Hello_swtr.sol github url` + `contract address`**

https://www.swisstronik.com/testnet2/dashboard#
