---
title: "Fundamentos de Modelagem e Projeto de Banco de Dados"
nav_order: 2
parent: "Modelagem e Banco de Dados"
---

Começamos discutindo as características fundamentais de um banco de dados. Um banco de dados é um sistema de armazenamento de informações organizado de maneira que um programa de computador possa selecionar rapidamente os dados desejados. Essa organização se dá em tabelas que possuem colunas e linhas para representar os registros. A característica marcante de um banco de dados é o seu alto nível de consistência, disponibilidade e integridade dos dados armazenados.

Mundo Fechado e mini-mundo são conceitos importantes ao tratar de banco de dados. O primeiro é a perspectiva que considera apenas o que está explicitamente presente no banco de dados como verdadeiro, tudo que não está presente é considerado falso ou desconhecido. Já o mini-mundo é a parte do mundo real que é modelada pelo banco de dados. Exemplo: Mini Mundo é um parque em miniatura brasileiro, localizado na cidade de Gramado, no Rio Grande do Sul, sendo uma das mais tradicionais atrações turísticas desta cidade. No parque existem cidades em miniatura, cerca de 24 vezes menor que o tamanho real.

No tópico de Álgebra Relacional, tratamos sobre uma linguagem de consulta procedural para bancos de dados relacionais. Nela, são usados operadores como união, intersecção, diferença, produto cartesiano, seleção e projeção para manipular conjuntos de dados.

A relação entre Álgebra Relacional e o projeto de banco de dados está em como os operadores da Álgebra são utilizados para modelar as consultas e operações que serão realizadas no banco de dados. É um pilar para o entendimento e utilização efetiva da SQL. #168

No que diz respeito à modelagem de banco de dados, essa é uma fase crucial para a estruturação eficiente dos dados. A modelagem auxilia na visualização da organização dos dados e seus relacionamentos, bem como ajuda a evitar redundâncias e inconsistências. Envolve conceitos como entidade, atributo e relação, que são representados em um Diagrama Entidade-Relacionamento (DER).

Ao falarmos de como "nasce" um banco de dados, exploramos o conceito de projeto de banco de dados. O projeto de um banco de dados começa com a definição dos requisitos do sistema e segue para a modelagem conceitual, onde os principais objetos de dados e seus relacionamentos são identificados.

No que tange ao projeto conceitual, essa é a fase de design de banco de dados onde o foco é na identificação das entidades, atributos e relacionamentos. O resultado é um modelo conceitual de alto nível que descreve estruturalmente um banco de dados sem considerar detalhes físicos.

Para entender o passo a passo do projeto conceitual, exemplificado o processo, que inclui a definição de entidades e relacionamentos, atributos, identificação de chaves primárias e restrições de integridade. #169

Na fase de implementação, abordamos o projeto lógico e físico. O projeto lógico traduz o modelo conceitual em um esquema de banco de dados em um modelo de dados, como o modelo relacional. Já o projeto físico se preocupa com a eficiência do banco de dados e leva em conta detalhes de como os dados serão fisicamente armazenados, como escolha de índices e estratégias de armazenamento.

Discutimos as fases de desenvolvimento de bancos de dados e aplicações, começando pela coleta e análise de requisitos, seguida pela modelagem conceitual, projeto lógico, projeto físico e a implementação. Cada fase tem um papel fundamental na garantia de que o banco de dados final atenda às necessidades do usuário e forneça um desempenho eficiente.
