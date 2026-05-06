# RangeStore.sol
RangeStore.sol
pragma solidity ^0.8.20;
contract RangeStore {
    uint public value;

    function set(uint x) public {
        require(x >= 10 && x <= 100, "Out of range");
        value = x;
    }
}
