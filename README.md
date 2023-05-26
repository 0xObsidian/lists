
## Multi-chain token list 
We collect many tokenlists from many providers, then we aggregate them by chains and tokens addresses. 
For each token we check whether it is listed in 2 or more tokenlists from different providers. If so, 
we add it to our trusted tokenlist.

## Providers
We collect tokenlists from github repos or open APIs from various platforms, currently:
- [CoinGecko](https://www.coingecko.com/)
- [1inch](https://app.1inch.io/)
- [Uniswap](https://uniswap.org/)
- [Sushiswap](https://www.sushi.com/)
- [OpenOcean](https://openocean.finance/)
- [QuickSwap](https://quickswap.exchange/#/swap)

## Chains with trusted tokens
Here are chains presented in our tokenlists with current token count. You can find out more in `/tokens` folder.
Token counts are approximate and may vary as providers update their tokenlists.
- Ethereum, 1567 tokens
- Bsc, 1076 tokens
- Polygon, 663 tokens
- Ftm, 320 tokens
- Avax, 318 tokens
- Arbitrum, 289 tokens
- Gnosis, 195 tokens
- Optimism, 140 tokens
- Cronos, 134 tokens
- Aurora, 133 tokens
- Moonriver, 101 tokens
- Moonbeam, 88 tokens
- Celo, 71 tokens
- Evmos, 49 tokens
- Boba, 40 tokens
- Fuse, 31 tokens

## Run aggregation script yourself
Install requirements
```$ pip3 install -r requirements.txt```
Run the script from repo root folder
```python3 aggregate_tokens.py```
## Generate readme.md based on aggregated data
```bash
python generate_readme.py
```
