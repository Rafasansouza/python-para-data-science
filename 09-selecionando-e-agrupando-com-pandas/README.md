# Resumo do Curso: Pandas - Selecionando e Agrupando Dados

## Introdução

Este curso foca em técnicas de seleção e agrupamento de dados utilizando a biblioteca Pandas em Python. O objetivo principal é capacitar você a manipular DataFrames para extrair informações relevantes e realizar análises exploratórias eficazes.

## Conteúdo Detalhado

### 1. Remodelando o DataFrame

*   **Leitura da Base de Dados:**
    *   Carregar os dados de um arquivo (ex: CSV) para um DataFrame Pandas.
    *   Exemplo:
        ```python
        import pandas as pd
        emissoes_gases = pd.read_csv('emissoes_gases.csv')
        ```
*   **Remoção de Informações Desnecessárias:**
    *   Identificar e remover colunas ou linhas que não serão utilizadas na análise.

### 2. Alterando o Formato do DataFrame

*   **Transformação de Colunas de Anos:**
    *   Converter as colunas de anos (ex: 1970, 1971, ..., 2021) em uma única coluna.
    *   Criar uma coluna separada para os valores de emissão correspondentes a cada ano.

### 3. Armazenando Informações das Colunas

*   **Identificação das Colunas a Manter:**
    *   Armazenar os nomes das colunas que contêm informações relevantes (ex: 'Nível 1 - Setor' até 'Produto').
    *   Exemplo:
        ```python
        colunas_info = list(emissoes_gases.loc[:,'Nível 1 - Setor':'Produto'].columns)
        ```
*   **Armazenamento das Colunas de Emissão (Anos):**
    *   Armazenar os nomes das colunas que representam os anos (ex: 1970 a 2021).
    *   Exemplo:
        ```python
        colunas_emissao = list(emissoes_gases.loc[:,1970:2021].columns)
        ```

### 4. Transformação com o Método `melt()`

*   **Utilização do Método `melt()`:**
    *   O método `melt()` é utilizado para transformar múltiplas colunas em duas colunas: uma para as variáveis e outra para os valores.
    *   Parâmetros:
        *   `id_vars`: Especifica as colunas que devem ser mantidas intactas.
        *   `value_vars`: Especifica as colunas que serão "derretidas" (transformadas em linhas).
        *   `var_name`: Define o nome da coluna que conterá os nomes das variáveis (ex: 'Ano').
        *   `value_name`: Define o nome da coluna que conterá os valores correspondentes (ex: 'Emissão').
    *   Exemplo:
        ```python
        emissoes_por_ano = emissoes_gases.melt(
            id_vars=colunas_info,
            value_vars=colunas_emissao,
            var_name='Ano',
            value_name='Emissão'
        )
        ```

### 5. Agrupamento de Dados

*   **Conceito de Agrupamento:**
    *   Agrupar dados permite agregar informações com base em categorias específicas, facilitando a análise e a identificação de padrões.
*   **Utilização do Método `groupby()`:**
    *   O método `groupby()` é utilizado para agrupar os dados com base em uma ou mais colunas.
    *   Exemplo:
        ```python
        # Agrupar por 'Nível 1 - Setor' e calcular a soma das emissões por ano
        emissoes_por_setor = emissoes_por_ano.groupby('Nível 1 - Setor')['Emissão'].sum()
        ```

## Conclusão

Ao final deste curso, você estará apto a remodelar DataFrames, transformar colunas e realizar agrupamentos de dados eficientes, permitindo análises exploratórias detalhadas e a extração de insights valiosos.