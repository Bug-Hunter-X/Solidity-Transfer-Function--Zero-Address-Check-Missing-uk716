# Solidity Transfer Function: Zero Address Check
This example demonstrates a common error in Solidity: failing to check if the recipient address is the zero address (0x0000000000000000000000000000000000000000) before transferring tokens.  Transferring to the zero address will result in irreversible loss of tokens. This repository shows the buggy code and a corrected version.

## Bug
The `transfer` function in `bug.sol` lacks a check for the zero address.

## Solution
The `transfer` function in `bugSolution.sol` incorporates a check to prevent sending tokens to the zero address.