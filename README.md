# pub_tlos_price
Publish the current TLOS price

## Requirements
CryptoCompare API Key (See [docs](https://min-api.cryptocompare.com/documentation))

## Overview
Python script that grabs the current TLOS/EOS pair price from Chainrift, then grabs the current EOS price from CryptoCompare (via unique API key), then prints all three prices:

- This unique key will only be allowed to claim tokens to YOUR account.  This way, if they key gets compromised it will do little or argueably "no" harm.

2.  Next, we create a separate wallet "claim" and provide ONLY this unique KEY

3.  Create a shell script "claimrewards.sh" to:
- Unlock this wallet
- Execute the claimrewards action
- Lock the wallet

4.  Setup a LOCAL USER cron job to run every hour.  (On TELOS, unclaimed rewards don't expire, so we don't need15 min so we get two chances to grab rewards during each reward period.worry about missing a claim)


## INSTALLATION
1.  Create new EOS KEY Pair (there are many ways to do this).

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwNDQ3NDE5OTYsLTE3NjYzOTU3NzldfQ
==
-->