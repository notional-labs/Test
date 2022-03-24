# Test Upgrade
This repo is for testing a chain upgrade on a single node local testnet

## Components

Bins folder contains pre-upgrade bin and upgrade bin

Post-upgrade.json contains all the queries and txs that will be executed orderly after the upgrade. Also each query/tx may comes with an expected result used to compare to the actual result got after running the query/tx. Same story with pre-upgrade.json

All the txs will be executed with a test account whose seed phrase is in test_account_seed.txt 

.test folder contains the chain data

## Running

Run test_upgrade.sh :

1. Run the chain with pre-upgrade bin, run all the txs/queries in pre-upgrade.json and assert their results.
2. Once chain hit upgrade height switch to upgrade bin to run the upgrade.
3. Run all the txs/queries in post-upgrade.json and assert their results.
