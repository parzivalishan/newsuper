Send Tokens to multiple accounts with your personal computer

## Adjusting Gas Fees

To change the gas fees for transactions, please modify the following parameters in the [code](https://github.com/parzivalishan/newsuper/blob/main/tools/mutlisender.py) on the line 55-58 , you would need to change the 0.51 and 40000 according to your needs and network conditions:

```python
# Estimate the gas for the transaction
gas_price = web3.to_wei('0.51', 'gwei')  # Gas price in gwei
gas_limit = 40000  # Gas limit
transaction_cost = gas_price * gas_limit

```

Make an Excel file with two colums named as Amount and Receiver like the following and add the data in it to use the multisend functionality of the tool




| Amount | Receiver |
|--------|----------|
| 100    | 0xAddress    |
| 200    | 0xAddress      |
| 150    | 0xAddress  |
