# truffle
truffle


     -- SimpleStorage.js

     pragma solidity ^0.5.0;

     contract SimpleStorage {
     uint val;
  
     function set(uint x) public {
        val = x;
     }

    function get() public view returns (uint) {
       return val;
    }
  
    }


 --- 1560882811_deploy.js
 
     var SimpleStorage = artifacts.require("SimpleStorage");

     module.exports = function(deployer) {
          deployer.deploy(SimpleStorage);
     };
