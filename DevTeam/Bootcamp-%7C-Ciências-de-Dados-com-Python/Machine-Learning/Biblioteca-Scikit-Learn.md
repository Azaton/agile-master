---
title: "Biblioteca Scikit Learn"
nav_order: 3
parent: "Machine Learning"
---

# Análise Preditiva com a Biblioteca Sklearn

Sklearn é uma biblioteca de código aberto voltada para a análise preditiva de dados. Ela é reutilizável em diversas situações e foi construída sobre os pacotes: NumPy, SciPy e matplotlib, tornando-a robusta e versátil.


Para exemplificar o uso da biblioteca Sklearn, vamos criar uma massa de dados com 200 observações. Esta massa de dados terá apenas uma variável preditora (x) e uma variável alvo (y). 

```python
# Importando a função para geração de dados
from sklearn.datasets import make_regression

# Parâmetros para a criação da massa de dados
n_samples = 200
n_features = 1
noise_level = 30

# Gerando a massa de dados
x, y = make_regression(n_samples=n_samples, n_features=n_features, noise=noise_level)
```


- noise: O parâmetro noise desempenha um papel crucial na determinação da variabilidade ou dispersão dos dados em relação a uma linha de tendência ideal.

- n_features = 1: Este parâmetro especifica o número de características (ou variáveis independentes) que cada observação terá.

- n_samples = 200: Este parâmetro determina o número total de observações (ou pontos de dados) que queremos no nosso conjunto de dados.

---

**Construção do Modelo de Machine Learning**:

Uma vez que temos os dados preparados, podemos prosseguir para a criação do modelo de aprendizado de máquina. No nosso exemplo, faremos uso da regressão linear disponível na Sklearn.

```python
# Importando o módulo necessário para a criação do modelo
from sklearn.linear_model import LinearRegression

# Criação do modelo de regressão linear
modelo = LinearRegression()
```

A função `LinearRegression()` é usada para criar o modelo. Se não indicarmos nenhum parâmetro específico ao chamar esta função, serão utilizadas as configurações padrão.

---

**Treinamento do Modelo**:

Com o modelo definido, o próximo passo é treiná-lo usando nossos dados. Isso é feito com o método `fit()`.

```python
# Treinando o modelo com os dados
modelo.fit(x, y)
```

Após a execução deste método, o objeto "modelo" estará treinado e pronto para fazer previsões.

---

# Método `predict()`:



O método `predict()` é um dos métodos centrais de muitos modelos de machine learning, especialmente em contextos de regressão e classificação. Depois de treinar um modelo, usamos o método `predict()` para obter previsões baseadas em novos dados que o modelo ainda não viu.

## Aplicação no Contexto

Considerando um modelo de regressão linear que foi treinado usando um conjunto de dados, composto por variáveis independentes \( x \) e uma variável dependente \( y \):

1. O método `predict()` toma um ou mais valores de \( x \) como entrada.
2. Ele então processa esses valores usando o modelo treinado e produz previsões correspondentes para \( y \).

**Exemplo**:

Imaginemos que temos um modelo de regressão linear treinado, chamado `modelo`. Para fazer previsões para um novo conjunto de valores \( x \) (por exemplo, chamado `x_novo`), faríamos o seguinte:

```python
y_predito = modelo.predict(x_novo)
```

Neste exemplo, `y_predito` conterá as previsões de \( y \) para cada valor em `x_novo`.

**Interpretação**:

Ao usar `predict()` em valores de \( x \), o que estamos fazendo é perguntar ao nosso modelo: "Dado o que você aprendeu durante o treinamento, qual seria sua estimativa ou previsão para \( y \) quando \( x \) é este valor específico?". O modelo então fornece uma resposta baseada no conhecimento que adquiriu durante o treinamento.

# Função plot()

O pacote `pyplot` faz parte da biblioteca `matplotlib`, que é uma das principais bibliotecas de visualização de dados em Python. 

**Explicação**:

- **plt.scatter()**: Esta função é usada para criar um gráfico de dispersão. No contexto de regressão, normalmente usamos isso para visualizar os dados originais (pontos reais).
  
- **plt.plot()**: Esta função é usada para desenhar linhas (ou marcar pontos) em um gráfico. No contexto da regressão, podemos usar isso para desenhar a linha de regressão (reta) para visualizar o ajuste do modelo aos dados.

**Exemplo de Código**:

Suponhamos que você já treinou um modelo de regressão linear e agora deseja visualizar os dados originais junto com a reta de regressão:

```python
plt.scatter(x,y)
plt.plot(x, modelo.predict(x), color='red', linewidth=3)
plt.show()
```



1. **`plt.scatter(x, y)`**: 
    - Esta função cria um gráfico de dispersão.
    - `x` e `y` são, respectivamente, os dados das variáveis independentes e dependentes.
    - O gráfico mostrará pontos individuais representando cada par de valores (x, y) nos dados originais.

2. **`plt.plot(x, modelo.predict(x), color='red', linewidth=3)`**: 
    - Esta função desenha uma linha no gráfico.
    - `x` são os valores da variável independente.
    - `modelo.predict(x)` retorna as previsões do modelo para cada valor de `x`. Essas previsões formarão a linha de regressão no gráfico.
    - `color='red'` especifica que a cor da linha será vermelha.
    - `linewidth=3` determina a espessura da linha, tornando-a mais grossa que o padrão.

3. **`plt.show()`**: 
    - Esta função exibe o gráfico. Até que essa função seja chamada, as alterações são apenas acumuladas e não são mostradas.

**Resultado Esperado**:

Ao executar este código:

- Um gráfico será exibido com pontos representando os dados originais (x, y).
- Uma linha vermelha (representando a reta de regressão) será traçada através dos pontos, mostrando a tendência dos dados conforme previsto pelo modelo.
- O contraste entre os pontos e a linha vermelha permitirá ao espectador avaliar visualmente o quão bem o modelo se ajusta aos dados.

Esse tipo de visualização é frequentemente utilizado para avaliar a qualidade do ajuste de um modelo de regressão linear aos dados. Se a linha vermelha passar próxima da maioria dos pontos, isso indica que o modelo tem um bom ajuste. Se houver muitos pontos distantes da linha, isso pode indicar problemas no ajuste do modelo ou na natureza dos dados.
