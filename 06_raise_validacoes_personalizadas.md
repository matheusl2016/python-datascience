# Raise: Validações e Exceções Personalizadas em Python

Neste módulo aprendi a usar o comando `raise` para criar minhas próprias mensagens de erro. Isso me permite validar os dados antes que eles sejam processados e evitar que o código rode com entradas erradas ou mal formatadas.

---

## Criando Exceções com `raise`

A função abaixo calcula a média de uma lista de notas, mas antes de fazer o cálculo, valida dois critérios:

1. A lista não pode ter mais de 4 notas  
2. Todos os elementos da lista devem ser numéricos (`int` ou `float`)

```python
def calcular_media(notas):
    if len(notas) > 4:
        raise ValueError("A lista não pode ter mais de 4 notas.")
    
    if not all(isinstance(n, (int, float)) for n in notas):
        raise TypeError("Todos os valores devem ser numéricos.")
    
    return sum(notas) / len(notas)

Exemplos de uso e testes:

Lista com mais de 4 notas (gera ValueError):
notas = [8, 7, 6, 5, 4]
media = calcular_media(notas)

  saída esperada:ValueError: A lista não pode ter mais de 4 notas.

Lista com tipo inválido (gera TypeError):
notas = [8, "9", 7]
media = calcular_media(notas)

  saída esperada: TypeError: Todos os valores devem ser numéricos.

Lista válida:
notas = [8.0, 9.5, 7.0]
media = calcular_media(notas)
print(media)  # 8.17


--Uso prático em projetos de dados:
-Esse tipo de validação é essencial quando estou lidando com:

Dados recebidos via formulários ou uploads
Planilhas e arquivos externos (como .csv)
Dados vindos de APIs públicas ou privadas
Qualquer sistema onde o usuário final pode enviar entradas inesperadas
