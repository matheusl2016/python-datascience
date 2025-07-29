# Bibliotecas, Funções e Estruturas Aninhadas em Python para Data Science

---

## Bibliotecas Python

Utilizei bibliotecas padrão do ecossistema Python para Data Science:

### matplotlib
Criação de gráficos, como barras, para visualização de médias de estudantes:

```python
import matplotlib.pyplot as plt

estudantes = ["João", "Maria", "José"]
notas = [8.5, 9, 6.5]

plt.bar(x=estudantes, height=notas)
plt.show()

Random:
from random import choice

estudantes = ["João", "Maria", "José", "Ana"]
estudante_sorteado = choice(estudantes)
print(estudante_sorteado)


#Funções:
Funções built-in (embutidas)
Utilizei funções como sum(), len(), type(), zip() e round() para cálculos rápidos e manipulações de dados.

Funções personalizadas
Criei funções reutilizáveis para automatizar tarefas como cálculo de média e classificação:
def media(lista):
    return round(sum(lista) / len(lista), 1)

Funções com retorno e múltiplas saídas:
def analisar_desempenho(notas):
    media = sum(notas) / len(notas)
    situacao = "Aprovado(a)" if media >= 6 else "Reprovado(a)"
    return media, situacao

Funções lambda e map():
Utilizei lambda para simplificar funções rápidas e map() para aplicar lógicas a coleções de dados:
qualitativo = 0.5
notas = [6.0, 7.0, 9.0, 5.5, 8.0]

notas_ajustadas = list(map(lambda x: x + qualitativo, notas))

Estruturas de Dados Aninhadas:
Aprendi a manipular listas compostas, listas de tuplas e dicionários de listas.
ex: lista de listas:

notas_turma = [
    [8.0, 9.0, 10.0],
    [9.0, 7.0, 6.0],
    [3.4, 7.0, 7.0]
]

Média com list comprehension:
medias = [sum(notas)/len(notas) for notas in notas_turma]

Filtro com compreensão condicional:
nomes = ["João", "Maria", "José"]
medias = [9.0, 7.5, 6.2]

bolsistas = [nome for (nome, media) in zip(nomes, medias) if media >= 8]

Dict Comprehension:
Transformei listas em dicionários organizados, úteis para consolidar dados em estruturas prontas para exportação:
dados = {
    "Estudantes": ["João", "Maria", "José"],
    "Notas": [[8, 9, 10], [7, 6, 8], [6, 7, 5]],
    "Média": [9.0, 7.0, 6.0]
}


