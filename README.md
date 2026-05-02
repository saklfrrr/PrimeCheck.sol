# PrimeCheck.sol
PrimeCheck.sol
pragma solidity ^0.8.20;
contract PrimeCheck {
    function isPrime(uint n) public pure returns(bool) {
        if(n < 2) return false;
        for(uint i=2;i*i<=n;i++){
            if(n % i == 0) return false;
        }
        return true;
    }
}
