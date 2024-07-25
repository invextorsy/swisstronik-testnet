# Swisstronik Testnet Task: Deploy a simple contract using Hardhat

## Setup Instructions

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
6. **Submit your `Hello_swtr.sol github url` + `contract address` in task: Deploy a simple contract using Hardhat**
