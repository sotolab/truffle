# truffle
truffle

Virsual Code
live server
prettier


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

  -- truffle-config.js

    networks: {
     development: {
      host: "127.0.0.1",     // Localhost (default: none)
      port: 8545,            // Standard Ethereum port (default: none)
      network_id: "*",       // Any network (default: none)
     },


