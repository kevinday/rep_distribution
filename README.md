The code in `rep_distribution.js` can be loaded into a geth console to initialize the rep contract.

Note that at the top of this file the line `primaryAddress = eth.accounts[0];`

If you'd like to initiate transactions from a different account, please change this.

Copying this into the console takes a very long time due to the size of the balance/address arrays. Instead, it is best to launch get with `--preload rep_distribution.js console`

To load the rep contract, call
`loadRepContract()`
Once the contract is ready to be used you will see ouptut in the console indicating the rep contract's address.

To initialize the contract with rep balances, call
`initializeRepBalances(0)`

To validate that the balances on the contract match the input, call
`validateBalances()`

If you'd like to validate your own balnce, you can do `repContract.balanceOf.call(address) / fxp`;
