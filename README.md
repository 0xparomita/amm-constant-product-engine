# AMM Constant Product Engine

This repository contains a high-quality, production-ready implementation of a Decentralized Exchange (DEX) core based on the Uniswap V2 architecture. It focuses on the mathematical heart of DeFi: the Constant Product Market Maker (CPMM).

## Core Mechanics
The engine ensures that the product of the reserves of two tokens remains constant during a swap:
$$x \cdot y = k$$
Where:
* $x$ is the reserve of Token A.
* $y$ is the reserve of Token B.
* $k$ is the constant product.



## Features
* **Automated Swaps:** Instant trades without a central order book.
* **Liquidity Provision:** Users can deposit token pairs to earn fees, receiving LP tokens in return.
* **Slippage Protection:** Internal checks to ensure trades don't exceed user-defined price impact limits.
* **Fee Collection:** Integrated 0.3% fee logic to incentivize liquidity providers.

## Getting Started
1. Deploy `AMM.sol` with two ERC20 token addresses.
2. Use `addLiquidity` to initialize the pool.
3. Call `swap` to exchange tokens instantly.

## License
MIT
