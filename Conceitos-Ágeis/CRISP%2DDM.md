---
title: "CRISP DM"
nav_order: 5
parent: "Conceitos Ágeis"
---

CRISP-DM, que significa **Cross-Industry Standard Process for Data Mining**, é uma metodologia amplamente utilizada para guiar o desenvolvimento de projetos de data mining (mineração de dados) e machine learning (aprendizado de máquina). O processo foi criado em 1996 por um consórcio liderado pela NCR e IBM, com o objetivo de estabelecer um padrão que fosse aplicável em diversas indústrias.

A metodologia CRISP-DM é composta por seis fases principais:

1. **Entendimento do Negócio (Business Understanding)**: Nesta fase, é essencial compreender os objetivos do negócio e os requisitos do projeto, transformando-os em uma definição clara do problema de mineração de dados. O entendimento do contexto e das prioridades do negócio é fundamental para o sucesso do projeto.

2. **Entendimento dos Dados (Data Understanding)**: Envolve coletar dados iniciais e explorar o conjunto de dados para familiarizar-se com ele, identificando problemas de qualidade e obtendo insights preliminares. Esta fase inclui a análise de dados para determinar sua adequação aos objetivos do projeto.

3. **Preparação dos Dados (Data Preparation)**: Nesta etapa, os dados brutos são transformados em um formato adequado para análise. Isso pode incluir a limpeza de dados, integração de múltiplas fontes de dados, seleção de variáveis relevantes e a formatação dos dados de acordo com as necessidades do modelo.

4. **Modelagem (Modeling)**: Envolve a aplicação de várias técnicas de modelagem para construir modelos preditivos. Nesta fase, é importante selecionar a técnica apropriada e ajustar os parâmetros do modelo para alcançar o melhor desempenho possível.

5. **Avaliação (Evaluation)**: Uma vez que os modelos são criados, eles precisam ser avaliados para garantir que atendam aos objetivos de negócio e que os resultados sejam robustos e interpretáveis. Isso pode incluir testes de validação cruzada, análise de precisão e revisão dos resultados em relação aos objetivos do negócio.

6. **Implementação (Deployment)**: A fase final envolve a implementação do modelo no ambiente de produção, onde ele pode ser usado para tomar decisões de negócio. Isso pode incluir a criação de relatórios, a integração do modelo em sistemas operacionais ou a criação de interfaces de usuário para facilitar o uso do modelo.


O CRISP-DM, o Método Científico e o Teste de Hipóteses são abordagens estruturadas que compartilham uma lógica comum de investigação e análise. Todos esses métodos são aplicáveis no contexto de Inteligência Artificial (IA), Data & Analytics, e Ciência de Dados, e podem ser inter-relacionados da seguinte forma:

### 1. **CRISP-DM e o Método Científico:**
O CRISP-DM pode ser visto como uma aplicação do Método Científico ao processo de análise de dados. Ambos seguem etapas semelhantes:

- **Observação e Entendimento do Problema:**
  - **Método Científico:** Começa com uma observação ou uma pergunta que leva à formulação de um problema ou hipótese.
  - **CRISP-DM:** Começa com o **Entendimento do Negócio**, onde os objetivos e questões de negócios são definidos.

- **Formulação de Hipóteses:**
  - **Método Científico:** Envolve a formulação de hipóteses que podem ser testadas.
  - **CRISP-DM:** Durante a fase de **Entendimento dos Dados** e **Preparação dos Dados**, hipóteses implícitas sobre a relação entre as variáveis e os resultados são consideradas.

- **Experimentação e Coleta de Dados:**
  - **Método Científico:** Testa as hipóteses coletando dados através de experimentos controlados.
  - **CRISP-DM:** Na fase de **Modelagem**, diferentes técnicas e algoritmos são aplicados para criar modelos que serão testados e avaliados.

- **Análise e Interpretação:**
  - **Método Científico:** Os resultados dos experimentos são analisados para confirmar ou refutar a hipótese.
  - **CRISP-DM:** Na fase de **Avaliação**, os modelos são avaliados para garantir que atendam aos objetivos do negócio.

- **Conclusão e Implementação:**
  - **Método Científico:** Conclui com a confirmação ou rejeição da hipótese, com base nos resultados, e pode levar a novas perguntas ou estudos.
  - **CRISP-DM:** Finaliza com a **Implementação** do modelo em um ambiente de produção, onde ele é utilizado para tomada de decisão.

### 2. **CRISP-DM e Teste de Hipóteses:**
O Teste de Hipóteses é uma técnica dentro do arcabouço do Método Científico, e é utilizado no CRISP-DM durante as fases de modelagem e avaliação:

- **Formulação de Hipóteses:** Durante a fase de **Modelagem**, hipóteses sobre a relação entre variáveis independentes e dependentes são formuladas. Essas hipóteses são testadas por meio de técnicas estatísticas ou algoritmos de aprendizado de máquina.

- **Teste e Validação:** Na fase de **Avaliação**, o Teste de Hipóteses é utilizado para determinar se os resultados do modelo são estatisticamente significativos e confiáveis. Isso pode envolver o uso de métricas como p-valores, intervalos de confiança, ou a validação cruzada dos modelos para garantir que eles generalizem bem aos novos dados.

- **Iteração:** Se as hipóteses são refutadas ou os modelos não atendem aos critérios de desempenho, o processo pode ser iterado, voltando às fases anteriores para reformular hipóteses ou ajustar o modelo.

### 3. **Inter-relação no Contexto de IA e Data Analytics:**
- **Data Analytics e IA:** Utilizam CRISP-DM para estruturar projetos de análise de dados, aplicando o Método Científico para investigar e extrair insights dos dados. O Teste de Hipóteses é uma ferramenta dentro desse processo, ajudando a validar descobertas e garantir que os modelos de IA sejam robustos e aplicáveis.

- **Exploração de Dados e Modelagem:** No contexto de IA, as fases de preparação de dados e modelagem no CRISP-DM são críticas, pois a qualidade dos dados e as hipóteses subjacentes afetam diretamente o desempenho dos modelos de IA. O uso rigoroso do Método Científico e do Teste de Hipóteses garante que as soluções de IA sejam baseadas em evidências e tenham um impacto positivo nos negócios.