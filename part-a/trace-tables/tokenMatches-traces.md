Timestamp: 2026-10-19 00:35:00 +01:00



| # | Kind    | given       | expected    | Predicted steps followed                                      | Predicted result |

|---|---------|-------------|-------------|---------------------------------------------------------------|------------------|

| 1 | Normal  | mango-tree  | mango-tree  | Steps 1, 2, 3, 4, 5, 6                                        | true             |

| 2 | Edge    | ""          | ""          | Steps 1, 2, 3, 4, 5, 6                                        | true             |

| 3 | Invalid | 42          | blue-bird   | Steps 1, 2, then early exit; steps 3, 4, 5, and 6 are skipped | false            |

