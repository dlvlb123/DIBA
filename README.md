All datasets are available at https://github.com/sjdseu/Real-CATS

## Feature List

### Transaction input features (`vin`)
1. `vin_count`: Number of input entries in the transaction.
2. `vin_total_value`: Total value of all transaction inputs.
3. `vin_mean_value`: Mean value of the transaction inputs.
4. `vin_max_value`: Maximum value among the transaction inputs.
5. `vin_min_value`: Minimum value among the transaction inputs.
6. `vin_value_variance`: Variance of the transaction input values.

### Transaction output features (`vout`)
7. `vout_count`: Number of output entries in the transaction.
8. `vout_total_value`: Total value of all transaction outputs.
9. `vout_mean_value`: Mean value of the transaction outputs.
10. `vout_max_value`: Maximum value among the transaction outputs.
11. `vout_min_value`: Minimum value among the transaction outputs.
12. `vout_value_variance`: Variance of the transaction output values.

### Target-address-related input features (`in`)
13. `in_count`: Number of inputs associated with the target address.
14. `in_total_value`: Total input value associated with the target address.
15. `in_mean_value`: Mean input value associated with the target address.
16. `in_max_value`: Maximum input value associated with the target address.
17. `in_min_value`: Minimum input value associated with the target address.
18. `in_value_variance`: Variance of the input values associated with the target address.

### Target-address-related output features (`out`)
19. `out_count`: Number of outputs associated with the target address.
20. `out_total_value`: Total output value associated with the target address.
21. `out_mean_value`: Mean output value associated with the target address.
22. `out_max_value`: Maximum output value associated with the target address.
23. `out_min_value`: Minimum output value associated with the target address.
24. `out_value_variance`: Variance of the output values associated with the target address.

### Ratio features
25. `in_count_ratio`: Ratio of `in_count` to `vin_count`.
26. `out_count_ratio`: Ratio of `out_count` to `vout_count`.
27. `in_mean_ratio`: Ratio of `in_mean_value` to `vin_mean_value`.
28. `out_mean_ratio`: Ratio of `out_mean_value` to `vout_mean_value`.
29. `in_value_ratio`: Ratio of `in_total_value` to `vin_total_value`.
30. `out_value_ratio`: Ratio of `out_total_value` to `vout_total_value`.

### Temporal and fee features
31. `fee`: Transaction fee.
32. `relative_time`: Time interval from the previous transaction.

### Address type count features
33. `in_P2PKH`: Number of P2PKH-type addresses in the input side associated with the target address.
34. `out_P2PKH`: Number of P2PKH-type addresses in the output side associated with the target address.
35. `in_P2SH`: Number of P2SH-type addresses in the input side associated with the target address.
36. `out_P2SH`: Number of P2SH-type addresses in the output side associated with the target address.
37. `in_P2WPKH`: Number of P2WPKH-type addresses in the input side associated with the target address.
38. `out_P2WPKH`: Number of P2WPKH-type addresses in the output side associated with the target address.
39. `in_P2WSH`: Number of P2WSH-type addresses in the input side associated with the target address.
40. `out_P2WSH`: Number of P2WSH-type addresses in the output side associated with the target address.

### Additional balance-related feature
41. `out_balance_ratio`: Ratio of the outgoing value to the current balance of the target address, used to measure the proportion of spending relative to the address balance.
