# Resumo do Curso NumPy: Análise Numérica Eficiente com Python

Este curso oferece um mergulho profundo na biblioteca NumPy, essencial para a análise numérica eficiente com Python. Através de exemplos práticos e exercícios, o curso capacita o aluno a manipular, analisar e visualizar dados de forma eficaz.

## Tópicos Abordados

*   **Introdução ao NumPy:**
    *   Visão geral da biblioteca NumPy e suas vantagens em relação às listas Python para operações numéricas.
    *   Instalação e configuração do ambiente para utilizar NumPy.
    *   Importação da biblioteca e verificação da versão instalada.

*   **Arrays NumPy:**
    *   Criação de arrays NumPy a partir de listas Python e outras estruturas de dados.
    *   Arrays de uma dimensão (vetores) e de múltiplas dimensões (matrizes).
    *   Atributos importantes dos arrays: `shape` (forma), `dtype` (tipo de dado), `size` (número de elementos) e `ndim` (número de dimensões).
    *   Indexação e fatiamento de arrays para acessar e modificar elementos.
    *   Cópia de arrays: `copy()` vs. visualizações (views).

*   **Operações com Arrays:**
    *   Operações aritméticas básicas: adição, subtração, multiplicação, divisão e potenciação.
    *   Operações com escalares e entre arrays de mesma forma.
    *   Funções matemáticas universais (ufuncs): `sin()`, `cos()`, `exp()`, `log()`, etc.
    *   Operações de comparação: `==`, `!=`, `>`, `<`, `>=`, `<=`.
    *   Operações lógicas: `&` (AND), `|` (OR), `~` (NOT).

*   **Funções Universais (ufuncs):**
    *   Conceito de funções universais e sua aplicação elemento a elemento em arrays.
    *   Ufuncs unárias (que operam em um único array) e binárias (que operam em dois arrays).
    *   Customização de ufuncs com `where` para aplicar operações condicionais.

*   **Broadcasting:**
    *   Entendimento do conceito de broadcasting e como ele permite realizar operações em arrays de diferentes formas.
    *   Regras de broadcasting e como NumPy as aplica automaticamente.
    *   Exemplos práticos de broadcasting para realizar operações vetoriais e matriciais de forma eficiente.

*   **Indexação Avançada:**
    *   Indexação booleana: seleção de elementos com base em condições lógicas.
    *   Fancy indexing: seleção de elementos utilizando arrays de índices.
    *   Combinação de indexação booleana e fancy indexing para seleções complexas.

*   **Álgebra Linear:**
    *   Operações com matrizes: produto escalar, produto vetorial, transposição.
    *   Resolução de sistemas lineares com `numpy.linalg.solve()`.
    *   Cálculo de autovalores e autovetores com `numpy.linalg.eig()`.
    *   Decomposição de matrizes: decomposição LU, decomposição QR.

*   **Números Aleatórios:**
    *   Geração de números aleatórios com `numpy.random` (inteiros, floats, distribuições).
    *   Controle de reprodutibilidade com `numpy.random.seed()`.
    *   Aplicações de números aleatórios em simulações e modelagem.

*   **Estatística:**
    *   Cálculo de estatísticas descritivas: média, mediana, desvio padrão, variância, percentis.
    *   Funções para calcular estatísticas ao longo de um eixo específico de um array.
    *   Histogramas com `numpy.histogram()` e visualização com Matplotlib.

*   **Tratamento de Dados:**
    *   Identificação de dados ausentes (NaN) com `numpy.isnan()`.
    *   Substituição de valores NaN por outros valores (zero, média, mediana).
    *   Remoção de linhas ou colunas com valores NaN.

*   **Visualização de Dados:**
    *   Integração com a biblioteca Matplotlib para criar gráficos a partir de dados NumPy.
    *   Criação de gráficos de linha, dispersão, barras e histogramas.
    *   Personalização de gráficos com títulos, rótulos, legendas e cores.

*   **Exemplos Práticos:**
    *   Análise de dados financeiros: cálculo de retornos, volatilidade e correlações.
    *   Processamento de imagens: manipulação de pixels, filtros e transformações.
    *   Simulações Monte Carlo: estimativa de probabilidades e resultados.

Este curso fornece uma base sólida para utilizar NumPy em projetos de análise de dados, ciência de dados, engenharia e outras áreas que envolvem cálculos numéricos e manipulação de dados. Ao final do curso, o aluno estará apto a:

*   Criar e manipular arrays NumPy de forma eficiente.
*   Realizar operações matemáticas, lógicas e estatísticas em arrays.
*   Aplicar funções universais (ufuncs) para realizar operações elemento a elemento.
*   Utilizar broadcasting para realizar operações em arrays de diferentes formas.
*   Realizar indexação avançada para selecionar elementos específicos de arrays.
*   Resolver problemas de álgebra linear com NumPy.
*   Gerar números aleatórios com NumPy e controlar a reprodutibilidade.
*   Tratar dados ausentes (NaN) em arrays NumPy.
*   Criar gráficos simples com Matplotlib a partir de dados NumPy.
*   Aplicar os conceitos aprendidos em exemplos práticos de análise de dados.