# Test Upgrade

bins folder contains pre-upgrade bin and upgrade bin

post-upgrade.json contains all the queries and txs that will be executed orderly after the upgrade. Also each query/tx may comes with an expected result used to compare to the actual result got after running the query/tx. Same story with pre-upgrade.json

all the txs will be executed with a test account whose seed phrase is in test_account_seed.txt 