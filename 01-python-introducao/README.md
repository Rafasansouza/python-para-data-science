# 🐍 Python: Resumo Completo

<div align="center">
  <img src="https://www.alura.com.br/artigos/python" alt="Python" width="400">
</div>

## 🌟 **Introdução**
Python é uma linguagem de programação **versátil** e **de alto nível**, criada por Guido van Rossum em 1991. É amplamente usada em:
```python
["Web", "IA", "Automação", "Ciência de Dados", "DevOps"]
```

### 🚀 **7 Motivos para Aprender**
1. Sintaxe simples e intuitiva
2. Comunidade ativa e apoio empresarial
3. Biblioteca padrão robusta (+113k pacotes no PyPI)
4. Multiplataforma (Windows/Linux/macOS)
5. Top 1 em Ciência de Dados (Python Developers Survey 2023)
6. Utilizada por Google, Instagram e NASA
7. Alta demanda no mercado (47% em Data Analysis)

---

## 📜 **História**
| Ano | Marco Histórico |
|------|-----------------|
| 1989 | Primeiras ideias de Guido van Rossum |
| 1991 | Lançamento oficial no CWI (Holanda) |
| 2000 | Sistema PEP para evolução da linguagem |
| 2023 | Versão 3.11 com ganhos de performance |

---

## ⚙️ **Instalação**
### Windows
```powershell
1. Baixe em python.org
2. Marque "Add Python to PATH"
3. Verifique no CMD:
   python --version
```

### Linux
```bash
sudo apt update && sudo apt install python3
python3 --version
```

---

## 🖥️ **IDEs Populares (2023)**
| Ferramenta | Uso | Popularidade |
|------------|-----|-------------|
| VS Code | Edição geral | 32% |
| PyCharm | Projetos complexos | 29% |
| Jupyter Notebook | Ciência de Dados | 6% |

---

## 🧮 **Tipos de Dados**
```python
# Exemplos Práticos
inteiro = 42             # int
texto = "Python"         # str
lista = [1, "a", True]   # list (mutável)
tupla = (1, 2)           # tuple (imutável)
dados = {"nome": "Ana"}  # dict
```

### 🔄 Conversão de Tipos
```python
idade = 18
idade_float = float(idade)  # 18.0
texto_numero = str(42)      # "42"
```

---

## 🎮 **Estruturas de Controle**
### Condicionais
```python
# if/elif/else
nota = 7.5
if nota >= 9:
    print("Excelente!")
elif nota >= 7:
    print("Aprovado")
else:
    print("Recuperação")

# Match (Python 3.10+)
match nota:
    case n if n >= 9: print("🌟")
    case n if n >= 7: print("✅")
    case _: print("⚠️")
```

### Loops
```python
# For
for i in range(1, 4):
    print(f"Execução {i}")

# While
contador = 0
while contador < 3:
    print(contador)
    contador += 1
```

---

## 📚 **Ecossistema Python**
### Principais Bibliotecas
| Categoria | Ferramentas |
|-----------|-------------|
| **Web** | Django, Flask, FastAPI |
| **Dados** | Pandas, NumPy, Matplotlib |
| **IA** | TensorFlow, PyTorch, Keras |
| **Automação** | Selenium, BeautifulSoup |

### PIP (Gerenciador de Pacotes)
```bash
pip install nome-pacote  # Instalação
pip freeze > requirements.txt  # Exportar dependências
```

---

## 🌐 **Quem Usa Python?**
| Empresa | Aplicação |
|---------|-----------|
| **Google** | Sistema de busca, YouTube |
| **Instagram** | Backend (14k+ endpoints) |
| **Netflix** | Sistema de recomendações |
| **NASA** | Cálculos espaciais |

---

## 📌 **Dica Final**
```python
# Primeiro Programa
print("Hello Python World! 🚀")

# Execute com:
# python seu_arquivo.py
```

> **Recursos**:  
> [Documentação Oficial](https://docs.python.org/3/) |  
> [Cursos Alura](https://www.alura.com.br) |  
> [Python Brasil](https://python.org.br)