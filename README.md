# Falcoin(UAED)

Upgradeable ERC20 token with freeze and gas-less transaction capability.

Contract conforms to [EIP-20](https://eips.ethereum.org/EIPS/eip-20), [EIP-712](https://eips.ethereum.org/EIPS/eip-712) and [EIP-2612](https://eips.ethereum.org/EIPS/eip-2612).

## Setup

To install with [Foundry](https://github.com/foundry-rs/foundry):

```sh
forge install
```

## Test

```sh
forge test
```

## Build

```sh
forge build
```

## Deploy

Deploy and verify sample token with Transparent Proxy [EIP-1967](https://eips.ethereum.org/EIPS/eip-1967):

```sh
export RPC=
export PK=
export ETHERSCAN_API_KEY=

forge script script/DeployStablecoin.s.sol:DeployStablecoinScript --rpc-url $RPC --private-key $PK --broadcast --verify --etherscan-api-key $ETHERSCAN_API_KEY -vvvv
```

