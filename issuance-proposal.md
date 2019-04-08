# Proposal for enabling issuance of fungible tokens in the Cosmos Hub

_*** WORK IN PROGRESS ***_

This proposal has been submitted on YYYY/MM/DD as proposal X on chain-id "cosmoshub-1".

## Executive summary
This proposal is a first step towards issuance of fungible tokens directly on the Cosmos Hub.

To ensure that the Cosmos Hub remains a pillar of trust, issuance of new tokens will granted on an individual basis through the addition of a new proposal type to the existing governance system.

## Background
In its current state, the primary utility of the Cosmos Hub is to demonstrate a working BPoS model and governance mechanisms.

The utility of the hub is expected to improve when IBC, one of the biggest value propositions of the Cosmos network, is implemented and enabled.

The work on IBC is on-going at https://github.com/cosmos/ics and is on track to eventually become a standard for interchain communication.

Regardless of the current IBC roadmap, fairly modest changes to cosmos-sdk will open up new possibilities for Cosmos Hub attracting value and real transaction volume to the network.

## Purpose
This governance proposal is _intended to gauge the interest_ of allowing issuance of fungible tokens directly in the Cosmos Hub, alongside its native ATOM token.

The advantages of implementing this proposal include:
* Lowers the "barrier to entry” for organizations and entities wishing to leverage the existing security and community that has been established on Cosmos Hub. Not all projects may want or need to maintain their own zone.

* Provides an immediate use for Cosmos Hub prior to the introduction of IBC.

* Attracts more value and transaction volume to the Cosmos Hub, thus increasing the value of ATOM.

The proposal restricts listing of new tokens to those that can pass the governance process. This acts as a quality filter for projects and strengthen the trust in the Cosmos Hub.

## Details
We propose that the governance proposal transactions are expanded with a new `ProposalKind`, e.g. `ProposalTypeAddToken`. This would allow new tokens to be introduced through standard governance without the need for network upgrades. The proposal should include an  issuer address from where new tokens can be minted and destroyed.

# Implementation
The development effort should be undertaken by one of the entities in the following, prioritized order
* Tendermint, Inc.
* 3rd party development team under a grant from the Interchain Foundation
* 3rd party development team financed by crowdfunding among the network participants

# Motivation
e-money.com has an immediate ambition to issue fungible tokens backed by fiat currencies in the Cosmos Network. The longer term goal is to launch a separate zone, but pending the arrival of IBC we expect that significant value can be created for the network by issuing directly on the Cosmos Hub.

Other projects will be able to use these tokens. Obvious use cases include services accepting fiat payments and wallet providers.

Validators and delegators will also benefit from the additional transaction volume on the network, which will lead to an increase in collected fees.

Full disclosure: e-money.com is part of the same group of companies as validator.network, the author of this proposal.

## Not in scope
Besides issuance, the token life cycle is specifically not in scope. The potential removal of an issued token from the Cosmos Hub is left for a future governance proposal, if deemed necessary.

## Voting options
| Vote             | Interpretation |
| ---------------- | -------------- |
| Yes              | I want the community to move forward with the idea of issuing custom tokens directly on the Cosmos Hub. |
| No               | I support issuance of custom tokens on the Cosmos Hub, but with a different implementation. |
| NoWithVeto       | Custom tokens should only originate in other zones and be present in the Cosmos hub through IBC. |

## Next steps
Following a successful (Yes) vote, the next steps are:
...