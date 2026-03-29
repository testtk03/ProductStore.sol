# ProductStore.sol
Base - Smart Contract Deployed by Remix ProductStore.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract ProductStore {
    struct Product {
        string name;
        uint price;
    }

    Product public product;

    function setProduct(string memory _name, uint _price) public {
        product = Product(_name, _price);
    }
}
