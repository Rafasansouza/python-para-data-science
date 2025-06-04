# 🐼 Pandas: Limpeza e Tratamento de Dados

Este repositório contém um resumo detalhado do curso **"Pandas: Limpeza e Tratamento de Dados"**, da [Alura](https://www.alura.com.br), ministrado pelo instrutor **Bruno Raphaell**.

O objetivo do curso é ensinar boas práticas de pré-processamento, preparando os dados para análises mais robustas ou aplicação de modelos de machine learning.

---

## 📚 Conteúdo Abordado

### 1. Strings Vazias

Aprendemos a identificar e remover strings vazias, que podem afetar estatísticas e resultados de análise.

```python
import pandas as pd

df = pd.DataFrame({'coluna': ['', 'valor1', '', 'valor2']})
df = df[df['coluna'] != '']
```

---

### 2. Modificação nos Tipos de Dados

Convertendo colunas para tipos adequados, permitindo cálculos e análises corretas.

```python
import pandas as pd

df = pd.DataFrame({'coluna': ['1', '2', '3']})
df['coluna'] = df['coluna'].astype(int)
```

---

### 3. Dados Duplicados

Identificação e remoção de registros duplicados para evitar distorções.

```python
import pandas as pd

df = pd.DataFrame({'coluna1': [1, 2, 3, 2], 'coluna2': [4, 5, 6, 5]})
df.drop_duplicates(inplace=True)
```

---

### 4. Dados Nulos

Tratamento de valores ausentes com preenchimento ou exclusão, evitando erros em análises.

```python
import pandas as pd
import numpy as np

df = pd.DataFrame({
    'coluna1': [1, 2, np.nan, 4],
    'coluna2': [4, 5, 6, np.nan]
})

df['coluna1'] = df['coluna1'].fillna(df['coluna1'].mean())
df['coluna2'] = df['coluna2'].fillna(df['coluna2'].mean())
```

---

### 5. Outliers

Detecção e tratamento de outliers com base no IQR (intervalo interquartil).

```python
import pandas as pd
import numpy as np

df = pd.DataFrame({'coluna': [1, 2, 3, 4, 500]})

q1 = df['coluna'].quantile(0.25)
q3 = df['coluna'].quantile(0.75)
iqr = q3 - q1

limite_inferior = q1 - 1.5 * iqr
limite_superior = q3 + 1.5 * iqr

df = df[(df['coluna'] >= limite_inferior) & (df['coluna'] <= limite_superior)]
```

---

## 💡 Conclusão

O curso forneceu uma base sólida sobre técnicas de limpeza de dados com Pandas, etapa essencial em qualquer projeto de ciência de dados. A manipulação adequada dos dados garante qualidade e precisão nas análises e modelos.

---

## 🚀 Tecnologias Utilizadas

- Python
- Pandas
- Jupyter Notebook (recomendado)

---

## 👨‍🏫 Instrutor

**Bruno Raphaell**  
Instrutor de Data Science na Alura

---

## 📎 Licença

Este repositório é apenas para fins educacionais, baseado em conteúdo da plataforma Alura.