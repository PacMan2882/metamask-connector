# metamask-connector

Metamask Connector is a tool to connect your metamask with your development environment, and let you say bye-bye to exposing your mnemonic or private key.

# Install

`npm install @PacMan2882/metamask-connector` 

or 

`yarn @PacMan2882/metamask-connector` to install the npm package.

# Usage
```
const { MetamaskConnector } = require("@PacMan2882/metamask-connector");
```
or

```
import { MetamaskConnector } from "@PacMan2882/metamask-connector";
```

```
let connector = new MetamaskConnector();
let signer = await connector.getSigner();
let signerAddr = await signer.getAddress();
```

# Test

There is a sample test hardhat project, just run `npm install` and `npx hardhat run scripts/deploy.ts` to make test in `example` folder.

# The idea

![](./metamask-connector.jpg)

# To be continue

- [x] Inject signer to ethers  
- [ ] Optimize the launch of the browser  
- [x] Optimize the webpage  
- [ ] Add support of other wallets
    - [ ] Coinbase Wallet
    - [ ] OKX Wallet
    - [ ] WalletConnect

## Special thanks
[metamask-client](https://github.com/PacMan2882/metamask-client)
