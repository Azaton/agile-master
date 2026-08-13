---
title: "Framework Luigi"
nav_order: 6
parent: "Machine Learning"
---

**Relação com as Bibliotecas Python**

[Luigi é um framework](https://luigi.readthedocs.io/en/stable/) Python focado na construção de pipelines de processamento de dados. Algumas das bibliotecas que podem ser facilmente integradas ao Luigi, incluem:

1. **pandas**: Utilizada para análise e manipulação de dados.
2. **NumPy**: Oferece suporte para operações matemáticas e manipulação de arrays.
3. **SQLAlchemy**: Uma ferramenta SQL e ORM (Object Relational Mapping) para conectar e manipular bancos de dados.
4. **Scikit-learn**: Uma das principais bibliotecas para machine learning em Python.
5. **boto3**: SDK da AWS para Python, permitindo interações com serviços como S3 e EC2.

**Natureza de Código Aberto**

Luigi foi desenvolvido como uma ferramenta de código aberto. Isso significa que qualquer pessoa pode acessar, modificar e distribuir seu código-fonte. Esta abertura facilita a colaboração, a contribuição da comunidade e a adaptação da ferramenta para necessidades específicas.

**Interface Gráfica e Visualização**

Uma das características distintas do Luigi é a sua interface visual. Esta interface permite aos usuários ver a estrutura e o status de suas tarefas e pipelines. Quando um pipeline Luigi é executado, ele cria uma representação visual das tarefas em forma de um DAG (Directed Acyclic Graph). 

Nesta visualização:

- Cada nó representa uma tarefa.
- As arestas representam as dependências entre as tarefas.
- As cores dos nós indicam o status da tarefa (por exemplo, verde para completo, vermelho para falha, etc.).

Esse suporte visual auxilia os desenvolvedores e equipes de dados a entender o fluxo de suas operações, identificar gargalos e monitorar o progresso das tarefas em tempo real.

![image.png](/.attachments/image-d5d1d5e0-1f27-4226-8497-8f6fa90125c8.png =700x)