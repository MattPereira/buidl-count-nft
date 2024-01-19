![OnlyBuidlors Thumbnail](https://only-buidlors.vercel.app/readme-logo.jpgs)

A dynamic SVG NFT project that uses chainlink functions to fetch off chain data from the BuidlGuidl API. All BuidlGuidl members with at least 1 published build are welcome to mint an NFT with a dynamic background color that changes based on the number of builds submitted!

## Getting Started
### Run It Locally
1. Clone the repo
```bash
git clone https://github.com/MattPereira/only-buidlors
```

2. Install the packages with yarn
```
yarn install
```

3. Start the project on localhost
```
yarn start
```

### Create Chainlink Functions Subscription
The deployment script is setup to automatically add any freshly deployed contract to a chainlink functions subscription, but the subscription itself must be created at functions.chain.link

Make sure to change the subscriptionId for all the different networks in the `HelperConfig.s.sol`

Also need to change `SUBSCRIPTION_ID` on the frontend homepage `index.tsx`

### Deploying Contracts
```
yarn deploy --network arbitrumSepolia
```
*Foundry `HelperConfig.s.sol` script is also setup to support deployment to eth-sepolia and mumbai



### Technology Stack

- Scaffold ETH 2
- Chainlink Functions
- Alchemy NFT API
