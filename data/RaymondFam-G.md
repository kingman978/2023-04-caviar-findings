## Combining for loops in `buy()` of PrivatePool
Like it has been implemented in [`sell()`](https://github.com/code-423n4/2023-04-caviar/blob/main/src/PrivatePool.sol#L328-L351), consider combining the two [for loops](https://github.com/code-423n4/2023-04-caviar/blob/main/src/PrivatePool.sol#L242) involving [`if (payRoyalties)`](https://github.com/code-423n4/2023-04-caviar/blob/main/src/PrivatePool.sol#L271) in [`buy()`](https://github.com/code-423n4/2023-04-caviar/blob/main/src/PrivatePool.sol#L211-L289) to save gas both on function calls and contract size. 