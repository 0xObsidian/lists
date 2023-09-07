
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
- Ethereum, 1474 tokens
- Bsc, 1009 tokens
- Polygon, 615 tokens
- Avax, 341 tokens
- Arbitrum, 308 tokens
- Ftm, 306 tokens
- Gnosis, 186 tokens
- Optimism, 156 tokens
- Aurora, 128 tokens
- Cronos, 103 tokens
- Moonriver, 90 tokens
- Moonbeam, 78 tokens
- Evmos, 46 tokens
- Celo, 37 tokens
- Boba, 35 tokens
- Fuse, 32 tokens
- Chains, 22 tokens
- Base, 19 tokens
- Zkevm, 16 tokens

## Run aggregation script yourself
Install requirements
```$ pip3 install -r requirements.txt```
Run the script from repo root folder
```python3 aggregate_tokens.py```
## Generate readme.md based on aggregated data
```bash
python generate_readme.py
```
