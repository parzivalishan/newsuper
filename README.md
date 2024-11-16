If you have any suggestions , you can create an issue [here]([url](https://github.com/parzivalishan/newsuper/issues)) or contact me : t.me/crypticishan 

---

#Whitelist function can be removed by adding a dead address (0x000000000000000000000000000000000000dead) to the whitelist.json file. It takes a few minutes to update in the frontend of the Launchpad.

0x000000000000000000000000000000000000dead makes the whitelist function = false, and then every wallet can be used on the launchpad, example:

```json
{
    "whitelistedAddresses": [
        "0x000000000000000000000000000000000000dead",
        "0x29de0cc374FC3432A9D9dE753BF12995E138DFf9",
        "0xE996BbDE2B2674bA8B4b3aae0E5C0E17e5B11dB9",
        "0x1736d80Db5da96ebA538Fb7CB90BF9d3eb0e0480"
    ]
}

```

if you remove anything from 0x000000000000000000000000000000000000dead , for example if i remove the last d from 0x000000000000000000000000000000000000dead . It becomes 0x000000000000000000000000000000000000dea and the whitelist function= true, then only wallets which are in the json are able to buy in the launchpad

---


 #maxBuyLimit function is used to implement the max buy for each wallet address. example-
```json
{
    "maxBuyLimits": {
        "0x000000000000000000000000000000000000dead": 300,
        "0xad3a5DdCe484251f8839f185896b14605b8dd340": 5,
        "0x29de0cc374FC3432A9D9dE753BF12995E138DFf9": 100,
        "0xE996BbDE2B2674bA8B4b3aae0E5C0E17e5B11dB9": 10
    }
}
```


this means that 0x000000000000000000000000000000000000dead overwrites every address, doesnt matter if the address is in the max buy limit or not .It would still have the the max limit of dead address which here is set to 300 

---

For the [Visit my repository] https://github.com/parzivalishan/newsuper/blob/main/tools/mutlisender.py , you would need to also use the excel sheet of this format [Visit my repository] https://github.com/parzivalishan/newsuper/blob/main/tools/transactions.xlsx for using the multisender feature from your local desktop . I am currently trying to fix the high gas issue on it but everything other than few dollars more on the gas fees works currently . I am in the process of fixing the high gas fees logic also . It would be fixed in the coming weeks . 
