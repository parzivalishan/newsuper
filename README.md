If you have any suggestions , you can create an issue [here]([url](https://github.com/parzivalishan/newsuper/issues)) or contact me : t.me/crypticishan 


#Whitelist function can be removed by adding a dead address(0x000000000000000000000000000000000000dead) to the whitelist.json file , it takes few minutes to update in the frontend of the Launchpad .


 #maxBuyLimit function is used to implement the max buy for each wallet address. example-
    "maxBuyLimits": {
        "0x000000000000000000000000000000000000dead" : 300,
        "0xad3a5DdCe484251f8839f185896b14605b8dd340": 5,
        "0x29de0cc374FC3432A9D9dE753BF12995E138DFf9": 100,
      "0xE996BbDE2B2674bA8B4b3aae0E5C0E17e5B11dB9": 10
    }
}

this means that 0x000000000000000000000000000000000000dead overwrites every address, doesnt matter if the address is in the max buy limit or not .It would still have the the max limit of dead address which here is set to 300 
