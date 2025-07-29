# Tratamento de Erros, Exceções e Boas Práticas em Python

Nesta parte do meu aprendizado, aprendi a lidar com exceções e a tornar o código mais seguro, previsível e profissional — especialmente importante em projetos de análise de dados, onde dados incompletos ou inconsistentes são comuns.

---

## Blocos `else` e `finally`

Adicionei lógica adicional quando o bloco `try` funcionava corretamente usando `else`, e um encerramento garantido do processo com `finally`.

```python
notas = {"Maria": [8.5, 9.0, 7.5]}

try:
    print(notas["Maria"])
except KeyError:
    print("Erro: Estudante não encontrado")
else:
    print("Consulta realizada com sucesso.")
finally:
    print("Consulta encerrada.")
