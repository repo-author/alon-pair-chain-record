# Independent re-reading of key transactions

Each transaction below was fetched again from a second RPC node (`api.mainnet-beta.solana.com`) and every token balance change and every
post-transaction SOL balance was compared with the figures used in the record. 'OK' means they agree to 1e-6 and the slot and block time are identical.

| Check | Transaction | Result | Detail |
|---|---|---|---|
| wallet acquires PUMP | [2uWXtQmE…](https://solscan.io/tx/2uWXtQmEm5c1XZwpw7KpkZUKwSPP6ECujcaeMjFiA5QKMgkpGaTwTGpRsXGXVLti7SzKkr4EUJYnx4EisZQRCJAA) | OK | max abs diff 0.00e+00; slot 469049741; 3 token balance changes, 13 SOL balances |
| BRACKET: creation | [3uFXpAKa…](https://solscan.io/tx/3uFXpAKa36ZLytLG6UZi2jH9QvrKabzGhnVdTrX4hjDwSWT4P7DuurhRZ2uugZ8m9nCF2E31p5iHPkDHo6hH3US2) | OK | max abs diff 0.00e+00; slot 469059390; 7 token balance changes, 33 SOL balances |
| BATON: creation | [q12aiQsj…](https://solscan.io/tx/q12aiQsjr5GzUnwAipJwDzwXcet594CK25w5uui7NKHupnk5MLGpB3EGVsDaT5eeCQxhYE41awPdCZUmEezTZxB) | OK | max abs diff 0.00e+00; slot 469059859; 1 token balance changes, 23 SOL balances |
| ALON: creation | [3QXZtFDd…](https://solscan.io/tx/3QXZtFDdmSnuGnztdRfXXJgXm5EdzTmryzwqX2Q9psTtDw7LtDo3x63NL95MsPB6skqxeHRYJfNPJ1J3WmErEog2) | OK | max abs diff 0.00e+00; slot 469060448; 1 token balance changes, 27 SOL balances |
| BATON: purchase by the wallet | [4btnhMHt…](https://solscan.io/tx/4btnhMHtyhqzYW4asxtcF8NPRp4Yc5A2HeB4uLSBY7dvpFU38omPRx1k1p1XMFPr3bVqzfnP99kwmbC6ca1w8F97) | OK | max abs diff 0.00e+00; slot 469059859; 5 token balance changes, 19 SOL balances |
| ALON: purchase by the wallet | [2JC7WWwr…](https://solscan.io/tx/2JC7WWwr8mpMDikyrE4fq5v64ZmLjPXfLMyrTsbKR9MMDZVjJYoBp1zFp4as2BcVaigtZzo4ANAv2B4U1cYSKAUk) | OK | max abs diff 0.00e+00; slot 469060448; 5 token balance changes, 19 SOL balances |
| BRACKET: migration | [2YrTdh9B…](https://solscan.io/tx/2YrTdh9BfpAy2byKdx4pGyNzMAcofpVqA1dJ1KcptrJ9Q2pEcDzfpX3wwk18eiqD8dvwtExHsawGbKt237Z8pvrk) | OK | max abs diff 0.00e+00; slot 469059392; 5 token balance changes, 28 SOL balances |
| BATON: migration | [4Lef1kYn…](https://solscan.io/tx/4Lef1kYnwznBt7Jv1qSuyHWKkJ33TYvzGhhPXzFun6L54KYrFDZKTeMpgvZS8s11VMfZpNfeAPipTK3MARpBNnJM) | OK | max abs diff 0.00e+00; slot 469059860; 5 token balance changes, 28 SOL balances |
| ALON: migration | [2zEEdLRJ…](https://solscan.io/tx/2zEEdLRJ71H8Yfrfq3Z64qa3tDiJ8N7UasJNbNoBv3R9u9s5ydHgnrKDuucutB6GQUq895fanvc3ox9grKx6mR5j) | OK | max abs diff 0.00e+00; slot 469060449; 5 token balance changes, 28 SOL balances |
| transfer of 999,000,000 ALON | [8sZSaHDh…](https://solscan.io/tx/8sZSaHDh4mp7nWGyhH7vuQn8eEVPPXTMTN7Wqv4MhjakbLC2niP6R5tc5hspRY6KW16vXot6GeEiJXXFPbn2Ua5) | OK | max abs diff 0.00e+00; slot 469060576; 2 token balance changes, 11 SOL balances |
| first ALON sale | [5q3Av4oY…](https://solscan.io/tx/5q3Av4oYuC1yFYuTpZnvAMJ7Q2j5uuiHsmeLmPFRheBrP13YUHi8iUkanTjPP44jiCU1mj5SzCkpThDwqY5Fb78m) | OK | max abs diff 0.00e+00; slot 469060599; 13 token balance changes, 49 SOL balances |
| last ALON sale | [2hu4G8WS…](https://solscan.io/tx/2hu4G8WS77sZpjtNCkzk23LRt4zxxZUiSPDmrmxtexQ6ewYJ12BGQVmDJkKR9GPjxomQzd9SeDxV9xDs32uw7hrw) | OK | max abs diff 0.00e+00; slot 469061423; 13 token balance changes, 49 SOL balances |
| largest ALON sale by SOL | [DgxDREAb…](https://solscan.io/tx/DgxDREAb6C4ahUdo7y7FLnygVEaVAM8kwh5oLD6xhLrwfecgjfiSnwXcgA4JWyDBEW5oxAhUW6JbQaawuELKF53) | OK | max abs diff 0.00e+00; slot 469060694; 13 token balance changes, 49 SOL balances |
| first transaction on the BRACKET pool after migration | [3YPA9vHH…](https://solscan.io/tx/3YPA9vHH9tGpi4iPxu2MSoeCA3BFw81Urykvwz4FJGrXgxySyX1PLy22cDe3nzndZdXzBpezY93q8FRYraqt4pEJ) | OK | max abs diff 0.00e+00; slot 469059397; 3 token balance changes, 15 SOL balances |
| 400th transaction on the BRACKET pool | [61WDCviu…](https://solscan.io/tx/61WDCviuyTFASp23ys4mE2VZ8FXrHpj35xhWmgbD4uv4JRGmv22nbZw8vfuftm4euQFXHFwCn4u71EjcZ2vKsma8) | OK | max abs diff 0.00e+00; slot 469060078; 11 token balance changes, 45 SOL balances |
