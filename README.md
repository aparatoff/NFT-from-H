# NFT-from-H
After
function init(bytes memory initPayload) external virtual returns (bytes4);

  function _isInitialized() internal view returns (bool initialized) {
    assembly {
      initialized := sload(_initializedSlot)
    }
  }

  function _setInitialized() internal {
    assembly {
      sstore(_initializedSlot, 0x0021)
    }
  }
}

++++

},
  "outputSelection": {
    "*": {
      "*": [
        "evm.bytecode",
        "evm.deployedBytecode",
        "devdoc",
        "userdoc",
        "metadata",
