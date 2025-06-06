[← All LSTs](../README.md)
# stKUB Proof of Reserves

## Methodology
stKUB LST is fully backed by staked KUB
> LST Total Supply = Minters + Delegated tokens + Unclaimed Rewards

### On-chain Delegations
KUB tokens are delegated directly to KUB validators via stKUB Minter on KUB. You can call the following methods to verify delegations and amounts.

- `getDelegatedAmount(address validator)` returns delegated balance
- `getUnclaimedRewards(address validator)` returns unclaimed delegation rewards

## Addresses

### stKUB Minters
| Network | Address | Explorer |
| -- | -- | -- |
| KUB | `0xea2a340f1ac58fba31bae7c5f31928ae6194c071` | [Explorer](https://kubscan.com/address/0xea2a340f1ac58fba31bae7c5f31928ae6194c071) |
