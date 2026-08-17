---
title: "Pequeno, Médio e Grande"
nav_order: 21
parent: "Conceitos Ágeis"
---

Dentro do contexto da **agilidade**, dividir um tema em **Pequeno (P), Médio (M) ou Grande (G)** é uma forma prática de estimar e estruturar os trabalhos a serem desenvolvidos dentro de um backlog. Essa categorização facilita a organização, o refinamento e a quebra de itens maiores em partes menores e entregáveis.

**1. Como dividir um tema em P, M ou G?**
-----------------------------------------

A abordagem mais comum para classificar o tamanho de um item é considerar **esforço, complexidade e incerteza**. Um critério simples pode ser:
*   **P (Pequeno):** Rápido de implementar, bem definido, baixo risco e esforço reduzido. Normalmente pode ser entregue dentro de um único sprint.
*   **M (Médio):** Exige mais esforço, pode ter dependências, precisa de mais discussão, mas ainda cabe dentro de um sprint ou ser finalizado com no máximo dois sprints.
*   **G (Grande):** Alto nível de complexidade, pode ter incertezas significativas e demanda refinamento. Não cabe em um único sprint e deve ser quebrado antes de ser levado para execução.

Uma boa prática é definir um tamanho máximo tolerável dentro do time. Por exemplo, se um item **G** está estimado para levar mais de 2-3 sprints, significa que precisa ser dividido antes de entrar na execução.

**2. Qual metodologia posso referenciar para P, M ou G?**
---------------------------------------------------------

Essa abordagem pode ser referenciada em diversas metodologias ágeis, mas algumas que lidam diretamente com granularidade de trabalho incluem:
*   **SAFe (Scaled Agile Framework):** Define granularidade em níveis como **Épicos → Features → Stories**, sendo que um Épico (G) precisa ser quebrado em Features (M) e, posteriormente, em Histórias (P).
*   **Scrum:** Trabalha com refinamento contínuo do backlog, onde **User Stories grandes precisam ser quebradas** antes de entrarem no sprint.
*   **Kanban:** Usa **Classes de Serviço** que podem determinar critérios para categorizar os itens e definir o fluxo de entrega.

**3. Como identificar o que é G para um Épico e o que pode ser M ou P, virando história?**
------------------------------------------------------------------------------------------

A estruturação pode ser feita seguindo a lógica:

![Define features and epics to organize backlog items - Azure Boards |  Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/boards/work-items/guidance/media/alm_pt_agile_wit_artifacts.png?view=azure-devops)

1.  **Se o tema é uma Iniciativa (Laranja), ele precisa ser refinado em Épicos (G - Roxo)**
    *   Uma **Iniciativa** representa um grande objetivo estratégico ou de produto, muitas vezes abrangendo múltiplos PIs (Program Increments) ou Releases.
    *   O próximo nível de detalhamento dentro da iniciativa é o **Épico**, que contém um conjunto de Features que sustentam esse objetivo.
2.  **Épico (G - Roxo)**
    *   Um **Épico** normalmente é um grande objetivo de negócio que não pode ser concluído em um único ciclo de desenvolvimento (como um PI no SAFe ou uma Sprint de um mês no Scrum).
    *   Para quebrá-lo, identifique as **entregas incrementais** que fazem sentido dentro do contexto e fornecem valor de forma iterativa.
3.  **Cada Épico (G) pode ser quebrada em Histórias (M)**
    *   As **Histórias** precisam ser independentes e entregáveis dentro de um sprint.
    *   Critérios de aceitação ajudam a validar se as histórias já podem ser desenvolvidas.
4.  **Cada História (M) pode ser quebrada em Tasks (P)**
    *   As **Tasks** representam atividades específicas necessárias para concluir uma história, como codificação, testes, revisão de código e deploy.
    *   As tarefas geralmente são estimadas em horas ou dias e são atribuídas a membros individuais do time.
