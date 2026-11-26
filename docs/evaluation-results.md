# Evaluation Results

The same 10 fictional test leads were evaluated with Prompt V1 and Prompt V2. Expected labels and score ranges were not included in the model input.

| # | Lead | Expected | Range | V1 result | V2 result |
|---:|---|---|---:|---|---|
| 1 | Olivia Bennett | hot | 9-10 | hot / 9 (in range) | hot / 9 (in range) |
| 2 | Ethan Walker | hot | 8-10 | hot / 9 (in range) | hot / 8 (in range) |
| 3 | Sophia Carter | hot | 8-9 | hot / 8 (in range) | hot / 8 (in range) |
| 4 | Mason Reed | warm | 5-6 | warm / 7 (out of range) | warm / 6 (in range) |
| 5 | Ava Mitchell | warm | 6-7 | warm / 6 (in range) | warm / 6 (in range) |
| 6 | Noah Foster | warm | 5-7 | warm / 7 (in range) | warm / 7 (in range) |
| 7 | Isabella Brooks | warm | 6-8 | warm / 5 (out of range) | warm / 6 (in range) |
| 8 | Lucas Gray | cold | 2-3 | cold / 2 (in range) | cold / 2 (in range) |
| 9 | Mia Richardson | cold | 1-2 | cold / 2 (in range) | cold / 2 (in range) |
| 10 | James Cooper | cold | 1-3 | cold / 2 (in range) | cold / 2 (in range) |

## Aggregate results

| Metric | V1 | V2 |
|---|---:|---:|
| Category agreement | 10/10 | 10/10 |
| Score within expected range | 8/10 | 10/10 |
| needs_review | 0 | 0 |
| Critical Hot → Cold | 0 | 0 |

## Observations

- V1 category predictions matched all 10 expected categories.
- V1 had two score-range mismatches: Mason Reed (7 vs. expected 5–6) and Isabella Brooks (5 vs. expected 6–8).
- V2 changed those scores to 6 and 6, respectively, while keeping all category predictions aligned with the expected labels.
- V2 achieved 10/10 score-range agreement on this dataset.

## Interpretation and limitation

This comparison indicates improved agreement with this particular synthetic test set after clarifying the scoring rubric. It does not demonstrate generalizable accuracy. The test set contains only 10 fictional examples generated with ChatGPT, and expected categories/ranges are predefined judgments. A larger, representative, independently labeled dataset would be needed for stronger evaluation.
