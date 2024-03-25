# Solana Meme Coin Creator + Toolkit

Create a Solana meme coin from start to finish with ease. Create token, get MarketID, create liquidity pool, burn LP, + bots to drive volume.  

* For full access to program, please contact @SolanaMemeDev on Telegram
* **UPDATE 3/24/24** The level of demand for this project has gone through the roof since word has spread what a useful tool this is. I've had multiple people tell me today that the program must not be real because it is too  **CHEAP**.  I contacted a few who have purchased it, and they also said I could easily double the price. Therefore, starting Monday March 25th, the price will be rising from 2 SOL to 4 SOL.    

Video of tool in action.  https://www.youtube.com/watch?feature=shared&v=aLEeoRuOioI
* In the video, it shows the cost to create a marketID and make the liquidity pool a 1.3 SOL.  This has been updated and the cost is now ~0.5 SOL using updated inputs.

```python
# .... SOLANA MEME COIN TOOLKIT -- V1.0 .....
# Created by ETHtricks 2024

# Main Menu - New Project

'Main Wallet - 3.131 SOL'

Select an Option (Blockchain Fees):
>
1. Create Token (0.01 SOL)
2. Create MarketID and Liquidity Pool (1.3 SOL + Liquidity)
3. Distribute Tokens (0.01 Sol)
4. Post Launch Options
5. Main Wallet Options


```


## Create Token

User friendly creation tool asks for token Name, symbol, number of tokens to mint, and image for token.  Also revokes mint authority.
```python
# Token Creator
Enter Name of Token:
>

Enter TICKER (3-7 Characters):
>

Number of Tokens to Mint (1000000000):
>

Path to Image for Token ('image.png'):
>
```

## Create Market ID and Liquidity Pool

Purchases a marketID to enable trading on your newly minted coin.

Default settings will pair 10 SOL with 80% of the token supply to create the liquidity pool.  These setting can be easily changed.  

Option to burn the LP tokens.  

```python

# Transfer Solana From Main Wallet
Number of SOL to add to liquidity pool? (Default: 10):
>

# Transfer Tokens From Main Wallet (%)
Percentage of total tokens to add to pool? (1-100 Default: 80):
>

# Burning the LP tokens adds legitimacy to your token.   
Do you want to burn the LP tokens created? (y/n)
>

......Creating Pool on Raydium...

......Success!
Your token is now listed and ready to be traded!

......Burning LP Tokens...

LP TOKENS BURNED!

TRANSACTION="34232543545234234235"
TOKEN_ADDRESS="address_from_mint"
LP_PAIR="lp_pair_created"
```
## Distribute Tokens



Create any number of fresh wallets and distribute a % of tokens to each new wallet.

* This option will spread distribution throughout a specified number of wallets. These wallets can then be used as "wash trading" wallets to increase the volume on your pair.  This greatly increases the visibility of your token on sites such as birdeye and photon. 


```python
# Create New Wallets
How many wallets would you like to create? (Default=10):
>

Creating Wallets....

..Wallet1 Created! 
    PublicKEY=abc123
    PrivateKEY=abc123abc123
..Wallet2 Created!
    PublicKEY=abc123
    PrivateKEY=abc123abc123
```

## Post Launch Options


It is essential to monitor your token once launched. 

* Example is using a token named "DogToes" with ticker "TOES". 

```python
# Launch Options

'TOES Price = $0.000000566' 
Select an option:
1. View Wallets and Balances
2. Increase the Volume!
3. Pump the Price!
4. Add more SOL to wallets
5. Dump ALL WALLETS (or trade LP if not burned)
```
* View Wallets and Balances

```python
# Wallets

Choose a Wallet: 
>
1. Wallet1
   TOES_Balance=123674122.00
   SOL_Balance=.0100087
   USD_Value=321.45

2. Wallet2
   TOES_Balance=437755732.00
   SOL_Balance=.00917558
   USD_Value=1056.89

3. Wallet3
   TOES_Balance=247355107.00
   SOL_Balance=.01074112
   USD_Value=644.42

```

Once a wallet is selected, Wallet Options will display.
```python
# Wallet Options

# Dumping a wallet sells all of the tokens in that wallet! 
# These tokens will be converted to SOL and added to your main wallet balance.
# Dump wallets from smallest to largest for best results.
# Wallet will be removed from your wallet list.

Wallet2
   TOES_Balance=437755732.00
   SOL_Balance=.00917558
   USD_Value=1056.89

Choose an option: 
>
1. Dump Wallet
2. Go Back
```
## Increase the Volume
Option 2 in post-launch options will send multiple small trades from your wallets to pump the amount of transactions on your token.  With the default settings, each wallet will sell ~0.1% - 0.3% of its tokens at random intervals. 

```python

```

## Pump the Price!

Option 3 in post-launch options will send 1 buy order from each of your wallets.  The default setting will buy your token with a random amount of SOL between 0.005 and 0.015.  This gives you volume and can give your price a boost if needed.  Increase these amounts for a bigger pump.
* BE SURE YOUR WALLETS HAVE ENOUGH SOL IF USING THIS OPTION

## Adding more SOL  to wallets
Will distribute a user defined amount of SOL from your main wallet into your token wallets.

## Main Wallet Options

```python
# Main Wallet Options

Select an Option:
>
1. Create a New Main Wallet
2. View Public Address and Check Balance
3. View Private Key
