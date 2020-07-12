# Primo passo di un branch & bound

Calcolo i rapporti tra profitti e pesi.

| Elemento | Profitti | Pesi | Rapporto |
|----------|----------|------|----------|
| A | 10 | 8 | 1.25 |
| B | 15 | 15 | 1.00 |
| C | 8 | 10 | 0.80 |
| D | 17 | 12 | 1.42 |
| E | 20 | 11 | 1.82 |

Ordino gli elementi per rapporto.

| Elemento | Profitti | Pesi | Rapporto |
|----------|----------|------|----------|
| E | 20 | 11 | 1.82 |
| D | 17 | 12 | 1.42 |
| A | 10 | 8 | 1.25 |
| B | 15 | 15 | 1.00 |
| C | 8 | 10 | 0.80 |

Prendiamo il branch in cui NON viene selezionato l'elemento E:  
l'upper bound di quel branch è dato dalla somma di tutti i profitti degli oggetti non ancora considerati.

```
D + A + B + C = 17 + 10 + 15 + 8 = 50
```

Non abbiamo ancora abbastanza informazioni per chiudere questo ramo; l'esplorazione deve procedere!
