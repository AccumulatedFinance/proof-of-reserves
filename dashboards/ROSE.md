[← All LSTs](../README.md)
# stROSE Proof of Reserves

## Methodology
stROSE LST is fully backed by staked ROSE
> LST Total Supply = Minters + Delegated tokens + Pending undelegations

### On-chain Delegations
ROSE tokens are delegated directly to Oasis validators on the Consensus layer via stROSE Minter on Oasis Sapphire. You can call the following methods to verify delegations and amounts.

- `getAllDelegations()` returns all validators to which ROSE tokens are delegated (in `0x` format; convert to `oasis1` format using bech32)
- `getDelegation(validator bytes21)` returns the number of shares, delegated to the validator
- Knowing the number of shares and the validator address, you can get the number of delegated tokens to this validator (using [Oasis Nexus API](https://nexus.oasis.io/v1/spec/v1.html) or validator page on [Oasisscan](https://www.oasisscan.com/validators))

### On-chain Pending Undelegations
- Pending undelegations take ~14 days and can be read using `getUndelegationReceipt(receiptId uint64)` method (first `receiptId = 4294967296`)

## Addresses

### stROSE Minters
Actual minter address(es) can be found here:<br />
[https://accumulated.finance/stake/rose](https://accumulated.finance/stake/rose)
