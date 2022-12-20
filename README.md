# Understanding Security Issues in the NFT Ecosystem

In our ACM CCS 2022 paper titled "[Understanding Security Issues in the NFT Ecosystem](4)", we perform the first systematic study of the emerging, multi-billion dollar Non-Fungible Token (NFT) ecosystem on top 8 NFT marketplaces.
We systematize the NFT ecosystem by identifying three major participating actors—marketplaces, external entities, and users.
In order to have an in-depth understanding of the market dynamics, we perform a large-scale data collection involving various sources, such as, the Ethereum mainnet, marketplace APIs, web crawling.
We then identify security and privacy issues, and design weaknesses surrounding the identified actors.
Lastly, we quantified the extent of the those threats on the data collected, whenever possible.

## Data

- The asset (e.g., collection name, asset URI, metadata URI, etc.) and event (e.g., mint, buy, sell, auction creation, placing of a bid, acceptance of a bid, transfer, etc.) data collected from the top 8 NFT marketplaces (OpenSea, Axie, CryptoPunks, Rarible, Superrare, Sorare, Foundation, and Nifty) are stored in their respective databases.
Since the OpenSea dataset contains events for the same set of assets, crawled three times, with a three-month interval between two subsequent crawls: in June 2021, September 2021, and finally in December 2021, therefore respective asset tables are appropriately timestamped: [https://zenodo.org/record/6526192](3)

- The `coins` database contains the Historical prices of the cryptocoins as provided by [CoinGecko](1): [https://zenodo.org/record/6526192](3)

- The `stats` database contains the availability of the source code of the token contracts in [Etherscan](2): [https://zenodo.org/record/6526192](3)

## Bibliography

```
@inproceedings{nft-study,
    author = {Dipanjan Das and Priyanka Bose and Nicola Ruaro and Christopher Kruegel and Giovanni Vigna},
    booktitle = {Proceedings of the ACM Conference on Computer and Communications Security (CCS)},
    title = {Understanding Security Issues in the NFT Ecosystem},
    year = {2022}
}
```

[1]: https://www.coingecko.com
[2]: https://etherscan.io
[3]: https://zenodo.org/record/6526192
[4]: https://arxiv.org/abs/2111.08893