// SPDX-License-Identifier: MIT
pragma solidity  0.8.26;

contract Calculator{
    //this function is to add num1, num2,
    function add(uint256 num1, uint256 num2) public pure returns (uint256) {
        return num1 + num2;
    }

// this function is to subtract num1, num2,
    function subtract(uint256 num1, uint256 num2) public pure returns (uint256) {
        require(num1 >= num2, "Result would be negative");
        return num1 - num2;
    }
// this function is to multiply num1, num2,
    function multiply(uint256 num1, uint256 num2) public pure returns (uint256) {
        return num1 * num2;
    }
// this function is to multiply num1, num2,
    function divide(uint256 num1, uint256 num2) public pure returns (uint256) {
        require(num2 != 0, "Cannot divide by zero");
        return num1 / num2;
    }

    function mod(uint256 num1, uint256 num2) public pure returns (uint256) {
        require(num2 != 0, "Cannot modulo by zero");
    return num1%num2;
    }
}
