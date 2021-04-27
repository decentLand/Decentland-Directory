# Contracts Documentation
This section is dedicated to document and explain the logic of decentland's smartweave contracts.

# Usernames
decentland's usernames represent unique limited type of tokens. To preserve usernames uniqueness and minter's username ownership across decent.land ecosystem, we have implemented the logic in a smartweave contract.

<h2>supported characters</h2>

username's characters are lower-case alphabetical only in other words, from a to z, or from character code 97 to 122.

<h2>minting stages and Tokens-Type</h2>

There are 3 (ALPHA, BETA, and GAMMA) usernames minting stages based on Arweave's network blockHeight. All the stages starts together, but in the last, only one stage will last, which is GAMMA (where usernames are common, not scarce).

Each stage define the allowed minimal username's length. For each username's length there is a type of tokens, and because the minimal username length is 1, and the maximal is 7, it means there are 7 types of tokens.

Each token (aka type of username) has a limited supply to ensure usernames rarety. The supply of each type is determined by the following formula: `x^y` where `x` represents the alphabetic characters number (fixed value, 26); and `y` evaluates to the number of username's length (1 to 7). Therefore, this is the list of each token's type and its total supply:
- "ichi": 26
- "ni": 626
- "san": 17576
- "shi": 456976
- "go": 11881376
- "roku": 308915776
- "shichi": 8031810176 

As said before, each minting stage support a limited username's length. it starts with the stage ALPHA, where it allows the mint of usernames of length 1 and 2, which means tokens `ichi` and `ni` . The next stage, BETA, the minimum username's length increases to 3 (`san` token type). 

And in the last one, GAMMA, `shi` tokens set the min length. After the 3 minting stages (which are time-limited / blockHeight), the final stage will be the only available one, where the username's minimum length increase to range(5, 7) or `go` to `shichi` tokens types.

It's worth to mentioned that the unminted tokens during the 3 minting stages will be locked forever in the contract. But as the last stage isn't blockHeight based, its tokens supply will be available as long there are users registering (the supply decrease by each new unique registration).

<h2>Tradability</h2>

decentland usernames will be tradable in the future, either Verto-supported or with a its own trading interface. Username minting is limited by one-per-address , which means when a user wants to switch (update) his/her username, they have to buy their wanted username from the market incase it was minted and available for sell.

The scarcity of username is proportional inversely to its length.

<h2>Switching</h2>

The user can hold as much as he wants (under the protocol rules) different type of tokens in his wallet. However, he/she has to choose a `currentUsername` or the displaying username. So when a user wants to update his username, he has to "switch" from his available tokens 
