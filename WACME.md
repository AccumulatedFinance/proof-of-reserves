# stACME (WACME) Liquid Staking
WACME liquid staking deployment

## stACME Minter(s)

| Network | Address | Explorer |
| -- | -- | -- |
| Ethereum | `0xdde19cf8bec23c2103f5ada61c83d5fd79e9714f` | [Explorer](https://etherscan.io/address/0xdde19cf8bec23c2103f5ada61c83d5fd79e9714f) |
| Arbitrum | `0xe54fb84a61583a4cc80878c396ebec588f84ff5d` | [Explorer](https://arbiscan.io/address/0xe54fb84a61583a4cc80878c396ebec588f84ff5d) |

**Important!** Each stACME token is independently managed on every chain. Do not bridge Ethereum stACME using Arbitrum bridge, you will get different token on the Arbitrum network.

## Staking Manager
There is no active staking manager, because liquid staking deposits are bridged directly into staking account using Accumulate Bridge.

## Staking Deployment
ACME accounts on Accumulate Network

| Name | Account | Explorer |
| -- | -- | -- |
| Staking account | `acc://accumulated.acme/staking` | [Explorer](https://explorer.accumulatenetwork.io/acc/accumulated.acme/staking) |
| Staking rewards | `acc://accumulated.acme/staking-rewards` | [Explorer](https://explorer.accumulatenetwork.io/acc/accumulated.acme/staking-rewards) |
| Protocol fees | `TBA` | `TBA` |
| stACME peg protection | `acc://accumulated.acme/peg-protection` | [Explorer](https://explorer.accumulatenetwork.io/acc/accumulated.acme/peg-protection) |
| Treasury | `acc://accumulated.acme/treasury` | [Explorer](https://explorer.accumulatenetwork.io/acc/accumulated.acme/treasury) |
