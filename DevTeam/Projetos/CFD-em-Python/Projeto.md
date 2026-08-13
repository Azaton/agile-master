---
title: "Projeto"
nav_order: 2
parent: "CFD em Python"
---

Durante os estudos e construção do código, utilizamos o Azure DevOps para mapear as atividades necessárias. As atividades foram dos mais diversos tipos, por exemplo, correções, pesquisas, histórias de usuário, Spike, levantamento e estudo de soluções.

Foi preciso reciclar os conhecimentos através de cursos:
- Lógica de Programação na Capgemini
- E-learning do LinkedIn "Descubra o Python".



O projeto foi escrito no Azure DevOps para organização e documentação, seguindo a estrutura [Iniciativa] Iniciativa Programação > [Projeto] - MVP Cumulative Flow Diagram.

Foram as features minimamente documentadas:

### Apresentar gráfico CFD numa tela para que o usuário
- Fazer o import das bibliotecas necessárias
- Uso da Matplotlib.pyplot para gerar os gráficos.
- Utilizados de Critérios de Aceite, História de Usuário.

### Estrutura de Arquivos e Pastas
- Banco de Dados e Cenários de Testes (Massa de Dados)
- Arquivos Py e HTML.
- Pasta 'static' para gerar a imagem local.
- Pasta ENV para Ambiente Virtual e instalar dependências do projeto.
- Tamplate chart.html, sendo a camada front do resultado do 'cfd_index.py'

### Configuração do Banco de Dados
- Massa de Dados CFD 12 Meses

### Configuração do Projeto Python no VS Code
- Criar ambiente Virtual "ENV" para o Python
- Instalação das libs gráficas.

### Criar um arquivo cfd_index.pye consumir os dados do banco
- Criar a estrutura do código
- Utilizado de lib para suportar arrays e funções matemáticas.

### Instalação do SQLite
- Baixar, organizar e instalar a versão do SQLite.
- Configurar a variável de ambiente.
- Criar o Banco e Tabela via script.
- Criar tabela e popular com dados para um CFD.