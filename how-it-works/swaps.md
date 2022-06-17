# Swaps

## How is the price decided?

We run an on-chain oracle that uses the average price on [Ubeswap](https://app.ubeswap.org/) over the previous 10 minutes.

## How are tokens swapped?

Running every order individually would be very expensive and inefficient, so what we do is put together the funds of everyone that has orders in the same pair and make one big swap instead of many small ones.

For example, if Alice wants to swap 2 cUSD for CELO every day and Bob wants to swap 5 cUSD for CELO every day, we will do one big swap of 7 cUSD and divide the obtained CELO proportionally between them. Both Alice and Bob can claimed their accrued CELO at any time.

## Who makes the swaps?

Anyone can make them! In practice, arbitrageurs are incentivized to do them for profit. Arbitrageurs search for inefficiencies in the markets to buy tokens slightly cheaper than normal by routing through all the exchanges on Celo. In the beginning the Mezumo team will run one basic bot that makes the swaps to bootstrap the project but we expect more players to join the fun over time.
