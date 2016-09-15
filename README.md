The code in `rep_distribution.js` can be pasted into a geth console to initialize the rep contract.

Note that at the top of this file the line `primaryAddress = eth.accounts[0];`

If you'd like to initiate transactions from a different account, please change this.

After copying into the console (this takes a long time due to the size of the address/balance arrays), do the following:

To load the rep contract, call
`loadRepContract()`
Once the contract is ready to be used you will see ouptut in the console indicating the rep contract's address.

To initialize the contract with rep balances, call
`initializeRepBalances(0)`

To validate that the balances on the contract match the input, call
`validateBalances()`

If you'd like to validate your own balnce, you can do `repContract.balanceOf.call(address) / fxp`;
