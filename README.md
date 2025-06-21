# Vault Setup

Restaking config: 4vvKh3Ws4vGzgXRVdo8SdL4jePXDvCqKVmi21BCBGwvn
Vault config: UwuSgAq4zByffCGCrWH87DsjfsewYjuqHfJEpzw1Jq3
TokenkegQfeZyiNwAJbNbGKPFXCWuBvf9Ss623VQ5DA

## Start Ledger


```
solana-test-validator \
    --clone TokenkegQfeZyiNwAJbNbGKPFXCWuBvf9Ss623VQ5DA \
    --clone ATokenGPvbdGVxr1b2hvZbsiqW5xWH25efTNsLJA8knL \
    --clone-upgradeable-program RestkWeAVL8fRGgzhfeoqFhsqKRchg6aa1XrcH96z4Q \
    --clone-upgradeable-program Vau1t6sLNxnzB7ZDsef8TLbPLfyZMYXH8WTNqUdm9g8 \
    --clone 4vvKh3Ws4vGzgXRVdo8SdL4jePXDvCqKVmi21BCBGwvn \
    --clone UwuSgAq4zByffCGCrWH87DsjfsewYjuqHfJEpzw1Jq3 \
    --url mainnet-beta \
    --slots-per-epoch 32 \
    --reset
```

## Create NCN

```
cargo r -p jito-tip-router-cli -- create-test-ncn --rpc-url "http://localhost:8899"
```




## Resources

- [PsyOptions Documentation](https://docs.psyoptions.io/)
- [PsyOptions Github](https://github.com/mithraiclabs/psyoptions)
