# ALON pair chain: on-chain record

A record of three Solana tokens created on 2026-11-13 and quoted in one another:
**ALON** (`8HQaU5pnmWgKijNsbcEDVQAvA6eNs577CRi8eqqqpump`) is quoted in **BATON** (`5pwkNm6E69DyvyTvMna9rM5sTFogbBLH3N3rvymPpump`), which is quoted in **BRACKET**
(`D2mA5zAMARotHeuGRPRCa1rZzWKrBAD9v2nntBt8pump`), which is quoted in the token PUMP. It covers the creation of each token, the first
purchase of each, the migration of each to its pool, the pools' contents at each step, the first 400
transactions on the BRACKET pool, and every transaction of the wallet that created the three tokens, up to
slot 469856591 (2026-11-15 20:03:26 UTC).

Everything here is reconstructed from the public Solana ledger. Every figure in the report is taken from a
transaction that is linked on solscan.io or listed by signature in the exhibits, so that it can be checked
without trusting this repository. The record states what the ledger shows. It draws no conclusion about
who controls any account or why any transaction was made.

## Contents

| File | What it is |
|---|---|
| `ALON_chain_record.md` | The report: accounts, how these tokens are priced, the sequence of 2026-11-13, the BRACKET pool's first transactions, the creating wallet's sales and other transactions, the state at the last slot read, method and limits |
| `verification.md` | 15 key transactions re-read from a second RPC node and compared |
| `fig_bracket_pool_pump.png` | PUMP held by the BRACKET pool, 20:25:50 – 20:33:08 UTC |
| `exhibits/accounts.csv` | Full addresses of the mints, curves, pools, vaults and programs |
| `exhibits/curve_transactions.csv` | Every successful transaction on the three bonding-curve accounts: one row per balance change |
| `exhibits/wallet_transactions.csv` | Every successful transaction of the creating wallet with its SOL and token balance changes |
| `exhibits/wallet_transfers.csv` | The wallet's plain transfers of SOL and tokens, with the counterparty account |
| `exhibits/pool_states_at_wallet_sells.csv` | Contents of the three pools and the resulting prices after each of the wallet's multi-pool sales |
| `exhibits/bracket_pool_first_1000_signatures.csv` | The first 1,000 successful signatures on the BRACKET pool, in block order |
| `exhibits/bracket_pool_first_400_transactions.csv` | The first 400 of those: fee payer, instructions, the pool's PUMP and BRACKET changes and balances |
| `exhibits/largest_token_accounts.csv` | The ten largest token accounts of each of the three tokens at the end of the record |

## How it was built

1. The curve and pool accounts of the three tokens were read from a Solana RPC node and decoded using the
   programs' public interface definitions (github.com/pump-fun/pump-public-docs).
2. All signatures of the three bonding-curve accounts and of the creating wallet were listed and each
   successful transaction fetched in parsed form.
3. The first 1,000 successful signatures of the BRACKET pool were listed in ascending order and the first
   400 transactions fetched. The pools' full histories (more than 200,000 signatures each within the first
   half hour) were not retrieved.
4. Every amount is the difference between the validator-recorded pre- and post-balances in the
   transaction, not a parser's interpretation. Instruction names are those the programs write to the log.
5. Pool prices are (quote tokens held + the pool's recorded virtual quote reserve) ÷ tokens held; the price
   of ALON in PUMP is the product of the three pool prices.
6. Key transactions were re-read from a second, independent node and compared.

Amounts in SOL marked "≈" convert PUMP at the rate of the wallet's own PUMP acquisition on 2026-11-13.
No US-dollar figures are given. Wallets are addresses, not people; one person may hold several, and some
are automated. No code is included; checking is done by reading the ledger.

## Checking it

Any figure can be checked by opening the linked transaction, or by reading the same signature from any
Solana node and comparing the pre- and post-balances.

## Corrections

If any figure here does not match the ledger, open an issue citing the transaction signature. The record
will be corrected and the correction noted.

## Licence

CC BY 4.0 (`LICENSE`).
