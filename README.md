# Peggy Front End

This is the repository for the Peggy Cellars frontend. Name of the repo can be considered a working title.

### Requirements:
- [ ] Landing page 
    - [ ] Design?
- [ ] Metamask integration
    - Signing and sending ethereum transactions to the [Peggy Contract](https://github.com/althea-net/peggy/blob/master/solidity/contracts/Peggy.sol)
    - Deriving a cosmos bech32 formatted pub key from metamask
    - Signing a cosmos sdk tx with metamask private key and verifying using that bech32 pub key
    - [Signing formatted cosmos transactions](https://medium.com/alpineintel/issuing-and-verifying-eip-712-challenges-with-go-32635ca78aaf): This is likely to be a bit of a challenge, but we want to offer an Ethereum native experience to users, meeting them where they are. See link for potential way this integration could work from the ETH signing side of things. As for key derivation ensuring that the sig will be valid on the Cosmos side we need to discuss more with @zmanian.
- [ ] Web3 query capability
    - See [`il-loss-charts`](https://github.com/PeggyJV/il-loss-charts#source-material) for some example queries
- [ ] Peggy Sommelier query capability
    - [CosmJS](https://github.com/cosmos/cosmjs) via GRPC query
- [ ] Peggy Sommelier tx generation, sign and send
    - [CosmJS](https://github.com/cosmos/cosmjs) tx sign mode tbd

The initial usecase we are planning to support is the [Stop Loss](./products/stop-loss) usecase.