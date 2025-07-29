# Fundamentos de Python – Variáveis, Condições e Repetições

Este material representa minha base prática com Python aplicada à análise de dados. Aqui mostro os principais comandos e estruturas que usei e como aplico em projetos reais.

## Variáveis e Tipos de Dados

Aprendi a declarar e manipular os principais tipos de dados em Python:

- **int**: números inteiros  
  `idade = 25`

- **float**: números decimais  
  `preco = 99.90`

- **str**: textos  
  `nome = "AFM Enterprise"`

- **bool**: valores booleanos  
  `ativo = True`

**Quando uso:** para carregar e armazenar valores vindos de arquivos CSV, planilhas ou APIs em projetos de análise.

---

## Estruturas Condicionais (`if`, `elif`, `else`)

Essas estruturas me permitem aplicar lógica aos dados.

```python
nota = 6.5

if nota >= 7:
    print("Aprovado")
elif nota >= 5:
    print("Recuperação")
else:
    print("Reprovado")
