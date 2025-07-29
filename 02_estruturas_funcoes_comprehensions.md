# Estruturas de Dados, Funções e Comprehensions em Python

Neste segundo módulo, aprofundei meu entendimento sobre como organizar e transformar dados usando estruturas compostas, funções reutilizáveis e técnicas de escrita mais eficiente de código.

## Estruturas de Dados

### Listas
Coleções mutáveis, ideais para armazenar sequências de dados.

frutas = ["maçã", "banana", "uva"]

Tuplas:
imutáveis, geralmente usadas para representar registros fixos.
  coordenadas = (23.5, 45.8)

Dicionários:
Estruturas de chave e valor. Muito úteis para organizar dados com rótulos.
  cliente = {"nome": "Carlos", "idade": 30}

Sets (Conjuntos):
Estruturas que não aceitam valores repetidos, úteis para filtrar ou agrupar.
  categorias = set(["A", "B", "A", "C"])  # {"A", "B", "C"}

Funções Personalizadas:
As funções me permitem encapsular lógicas específicas e reutilizá-las ao longo do projeto.
  def calcular_media(valores):
    return sum(valores) / len(valores)
      #Quando uso: para aplicar transformações, cálculos ou validações em colunas de dados, como verificar valores nulos ou normalizar colunas numéricas.



List e Dict Comprehensions:
Uma forma compacta e eficiente de criar listas ou dicionários.

Lista (List Comprehension):
quadrados = [x**2 for x in range(5)]  # [0, 1, 4, 9, 16]

Dicionário (Dict Comprehension):
dobros = {x: x*2 for x in range(3)}  # {0: 0, 1: 2, 2: 4}
  #Quando uso: para criar colunas derivadas com base em regras, simplificar filtros e acelerar o processamento de listas ou DataFrames.
