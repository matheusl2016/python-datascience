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
