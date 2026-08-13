---
title: "Biblioteca Pandas"
nav_order: 2
parent: "Machine Learning"
has_children: true
---

A biblioteca Pandas é uma das mais importantes ferramentas na linguagem Python para manipulação e análise de dados. Devido à vastidão de suas funcionalidades, muitos usuários não estão plenamente cientes de todas as suas capacidades. Comparada frequentemente ao Microsoft Excel devido à sua facilidade em manipular dados estruturados, a Pandas permite construir, modificar e analisar grandes conjuntos de dados de maneira eficiente.

**Características Principais**:

1. **Manipulação de Dados Estruturados**: Assim como no Excel, a Pandas oferece funções para manipulação de tabelas, permitindo operações como filtragem, ordenação e agregação.
   
2. **Análise Inteligente de Dados**: A biblioteca fornece métodos para análises estatísticas, tratamento de valores faltantes e visualização gráfica integrada.

3. **Interoperabilidade com Outras Bibliotecas**: Além da Pandas, existem outras bibliotecas populares como OpenCV (para processamento de imagens), Scikit-Image (manipulação de imagens) e Pillow (processamento de imagens). A Pandas se integra bem a muitas destas, facilitando a análise conjunta.

**Funções Detalhadas**:

1. **df.shape**: 
   - **Descrição**: Retorna uma tupla representando a dimensionalidade do DataFrame.
   - **Exemplo**:
     ```python
     import pandas as pd
     data = {'A': [1, 2], 'B': [3, 4]}
     df = pd.DataFrame(data)
     print(df.shape)  # Saída: (2, 2)
     ```

2. **df. info**
   - **Descrição**: Fornece um resumo conciso do DataFrame, incluindo a quantidade de valores não nulos e tipos de dados.
   - **Exemplo**:
     ```python
     df.info()
     ```

3. **df.isnull().sum()**:
   - **Descrição**: Retorna a soma de valores faltantes para cada coluna.
   - **Exemplo**:
     ```python
     print(df.isnull().sum())
     ```

4. **df['setor'].unique()**:
   - **Descrição**: Retorna valores únicos de uma coluna.
   - **Exemplo**:
     ```python
     df['setor'].unique()
     ```

5. **df['setor'].value_counts().plot(kind='bar')**:
   - **Descrição**: Conta a ocorrência de cada valor único em uma coluna e exibe um gráfico de barras.
   - **Exemplo**:
     ```python
     df['setor'].value_counts().plot(kind='bar')
     ```

6. **df.describe()**:
   - **Descrição**: Fornece estatísticas descritivas do DataFrame, como média, mediana, mínimo, máximo e quartis.
   - **Exemplo**:
     ```python
     df.describe()
     ```

----

# detalhes das Funcionalidades

**1. df.shape**:
- **Descrição**: Esta propriedade retorna uma tupla que representa a dimensionalidade do DataFrame. Especificamente, mostra o número de linhas e colunas.
- **Uso Profundo**: Saber a dimensão de um DataFrame é útil principalmente na fase inicial da análise de dados, para se ter uma noção do tamanho do conjunto de dados com o qual você está trabalhando. 

**2. df einfo**:
- **Descrição**: Esta função fornece um resumo conciso do DataFrame. Mostra informações sobre os tipos de dados, valores não nulos e memória usada.
- **Uso Profundo**: `df.info()` é vital durante a fase exploratória de análise de dados. Ele permite que você rapidamente identifique colunas que possam ter valores faltantes e compreenda os tipos de dados de cada coluna, ajudando na tomada de decisões sobre limpeza e transformação de dados.

**3. df.isnull().sum()**:
- **Descrição**: A combinação de `isnull()` e `sum()` permite contar a quantidade de valores faltantes em cada coluna.
- **Uso Profundo**: Identificar valores faltantes é crucial na pré-processamento de dados, pois eles podem afetar os resultados da análise. Sabendo onde estão os valores faltantes, você pode decidir imputá-los, removê-los ou investigar sua origem.

**4. df['setor'].unique()**:
- **Descrição**: Esta função retorna os valores únicos de uma coluna específica.
- **Uso Profundo**: Especialmente útil quando você deseja entender a diversidade de valores em uma coluna categórica. Por exemplo, saber todos os setores únicos em um conjunto de dados de empresas pode ajudar a orientar análises setoriais.

**5. df['setor'].value_counts().plot(kind='bar')**:
- **Descrição**: Esta cadeia de funções conta a ocorrência de cada valor único em uma coluna e, em seguida, exibe esse conteúdo em um gráfico de barras.
- **Uso Profundo**: Visualizar a distribuição de valores categóricos é uma ferramenta poderosa. Por exemplo, se você quiser visualizar a distribuição de empresas por setor, esta função permitirá que você identifique rapidamente setores dominantes ou sub-representados.

**6. df.describe()**:
- **Descrição**: Esta função fornece estatísticas descritivas das colunas, mostrando medidas como média, mediana, valor mínimo, valor máximo, e os quartis.
- **Uso Profundo**: Durante a análise exploratória, `df.describe()` oferece um resumo estatístico que pode ajudar a identificar tendências, outliers ou necessidades de normalização. Por exemplo, uma média significativamente diferente da mediana pode indicar a presença de outliers que estão afetando a distribuição.
