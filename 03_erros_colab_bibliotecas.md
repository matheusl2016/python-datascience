``markdown

## Tratamento de Erros

Utilizo `try`, `except` e `finally` para tornar meu código mais robusto e à prova de falhas comuns.

```python
try:
    resultado = 10 / 0
except ZeroDivisionError:
    print("Divisão por zero não é permitida.")
finally:
    print("Fim do cálculo.")
