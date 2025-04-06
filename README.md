// SPDX-License-Identifier: MIT  
pragma solidity ^0.8.0;  
contract BismillahValidator {  
  function start(bytes32 bismillahHash) public pure returns (bool) {  
    require(bismillahHash == keccak256("بِسْمِ اللهِ"), "HC: Start with Bismillah");  
    return true;  
  }  
}