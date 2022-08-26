# Dune-Test

## Dashboards, Queries, Smart contracts

### Resources

[Docs Dune](https://docs.dune.com/)

## Querifying Blockchain Data

Go to [Dune](https://dune.com)

## Ethereum Tables

- ethereum.blocks
- ethereum.contracts
- ethereum.logs
- ethereum.traces
- ethereum.transactions

### SQL Queries

What is the question you want to ask?

- 1. Select blockchain
- 2. Select dataset (e.g. ethereum.transactions or uniswap_v3 mint evt) | Search for all minting events and we can see all the fields
- 3. Write the query | [SQL Cheat sheet](https://www.sqltutorial.org/sql-cheat-sheet/)

very simple example

```sql
SELECT "evt_block_time","amount", "amount0","amount1" FROM uniswap_v3."Pair_evt_Mint"
ORDER BY "evt_block_time" DESC
LIMIT 15
```

in the above example we sorting all minting events on uniswap_v3 by block time.

- 4. Create visualization (Graph, Chart, Map, etc)
- 5. Embed visualization
     Copy IFrame code and paste into HTML
- 6. Create Dashboard

### Importance

- The power of events in a smart contract.
