[← All LSTs](../README.md)
# stROSE Proof of Reserves

## Methodology
Each stROSE is fully backed by staked ROSE.
> LST Total Supply = Minters + Delegated tokens + Pending undelegations

### On-chain Delegations/Undelegations
ROSE tokens are delegated directly to Oasis validators on the Consensus layer via stROSE Minter on Oasis Sapphire. You can call the following methods to verify delegations and amounts.

- `getAllDelegations()` returns all validators to which ROSE tokens are delegated (in `0x` format; conversion to `oasis1` format using bech32)
- `getDelegation(validator bytes21)` returns number of shares, delegated to the validator
- Knowing the number of shares and the validator address, you can get the number of delegated tokens to this validaor (using [Oasis Nexus API](https://nexus.oasis.io/v1/spec/v1.html) or validator page on [Oasisscan](https://www.oasisscan.com/validators))
- Pending undelegations take ~14 days and can be read by reading undelegation receipts using `getUndelegationReceipt(receiptId uint64)` method

## Addresses

### stROSE Minter(s)

| Network | Address | Explorer |
| -- | -- | -- |
| Oasis Sapphire | `0xb9c0df6e5df4e5eabb824d66c764dee0b889d574` | [Explorer](https://explorer.oasis.io/mainnet/sapphire/address/0xb9c0df6e5df4e5eabb824d66c764dee0b889d574) |