---
title: "LeSS"
nav_order: 1
parent: "Ágil em Escala"
---

# Large-Scale Scrum (LeSS)

## O que é

**Large-Scale Scrum (LeSS)** é um framework ágil criado para escalar o Scrum de uma única equipe para **múltiplas equipes trabalhando sobre um mesmo produto**.

A proposta central do LeSS é preservar os princípios do Scrum mesmo em contextos maiores, evitando adicionar camadas excessivas de gestão, papéis intermediários e estruturas organizacionais complexas.

Em vez de criar vários backlogs, vários Product Owners ou estruturas independentes por equipe, o LeSS busca manter uma visão integrada do produto por meio de:

- **um único Product Owner**;
- **um único Product Backlog**;
- **um produto compartilhado**;
- **uma Sprint comum** entre as equipes;
- coordenação baseada em colaboração direta e transparência.

O objetivo é reduzir complexidade organizacional e evitar que os times se transformem em silos especializados ou estruturas independentes que perdem a visão do produto como um todo.

## Tipos de LeSS

O framework possui duas configurações principais.

### Basic LeSS

O **Basic LeSS** é voltado para organizações com aproximadamente **2 a 8 equipes** trabalhando de maneira colaborativa sobre o mesmo produto.

Em geral, isso representa algo em torno de **10 a 50 pessoas**, embora o foco do framework esteja mais na estrutura dos times e do produto do que em um número rígido de profissionais.

A configuração mantém a estrutura do Scrum bastante enxuta, buscando evitar a criação de níveis adicionais de coordenação ou gestão.

### LeSS Huge

O **LeSS Huge** é destinado a contextos com **mais de 8 equipes**, podendo ser aplicado em organizações significativamente maiores.

Nesse cenário, surge o conceito de **Requirement Areas**, que agrupa partes relevantes do produto, e podem existir **Area Product Owners** responsáveis por apoiar a gestão dessas áreas.

Mesmo com essa estrutura adicional, continua existindo uma visão de produto integrada e um Product Owner responsável pelo produto como um todo.

## Princípios centrais

### Foco no produto como um todo

As equipes devem trabalhar olhando para o **produto completo**, e não apenas para componentes técnicos, sistemas isolados ou subprodutos locais.

Isso reduz a tendência de formar silos organizacionais em que cada equipe otimiza somente sua própria parte do sistema.

### Transparência

LeSS enfatiza transparência sobre:

- utilização real do produto pelo cliente;
- estado do código e da solução;
- dependências;
- impedimentos;
- gargalos organizacionais;
- progresso real da entrega.

A transparência cria as condições necessárias para inspeção e adaptação.

### Melhoria contínua

O framework preserva o empirismo do Scrum: ciclos curtos de trabalho, inspeção frequente dos resultados e adaptação contínua.

A melhoria não se restringe ao produto. O próprio desenho organizacional, os processos e as relações entre os times também devem evoluir conforme os problemas se tornam visíveis.

### Scrum em escala com o mínimo de estruturas adicionais

Uma característica importante do LeSS é a busca por **escalar o Scrum reduzindo complexidade**, em vez de responder ao crescimento criando novas camadas de controle.

Por isso, o framework procura manter regras e artefatos mínimos e incentivar comunicação direta entre as equipes.

## Estrutura conceitual

Uma forma simplificada de visualizar o LeSS é:

```text
                    PRODUTO
                       ↓
               Product Owner
                       ↓
              Product Backlog
                       ↓
        ┌──────────────┼──────────────┐
        ↓              ↓              ↓
     Equipe A        Equipe B       Equipe C
        └──────────────┼──────────────┘
                       ↓
                 Sprint comum
                       ↓
              Incremento integrado
```

As equipes não possuem produtos independentes. Todas contribuem para um **mesmo incremento integrado do produto**.

## LeSS e o Scrum tradicional

LeSS não procura substituir o Scrum. Sua proposta é aplicar os mesmos fundamentos do Scrum em uma escala maior.

No Scrum tradicional, normalmente existe:

```text
1 Product Owner
1 Product Backlog
1 Scrum Team
1 Sprint
1 Incremento
```

No LeSS, a lógica passa a ser:

```text
1 Product Owner
1 Product Backlog
Vários times
1 Sprint compartilhada
1 Incremento integrado
```

A principal mudança está, portanto, na quantidade de equipes que trabalham sobre o produto — não na criação de vários sistemas paralelos de gestão.

## O problema que o LeSS busca resolver

Quando organizações crescem, é comum surgirem estruturas como:

- equipes organizadas por componente;
- múltiplos backlogs desconectados;
- vários níveis de gestão;
- dependências excessivas entre áreas;
- handoffs;
- filas de aprovação;
- equipes otimizando apenas metas locais.

LeSS procura reduzir esses efeitos mantendo o trabalho orientado ao produto e aumentando a capacidade das equipes de entregar valor de ponta a ponta.

## Relação com outros frameworks de agilidade em escala

LeSS pertence ao conjunto de abordagens utilizadas para escalar princípios ágeis em organizações com múltiplas equipes.

Ele se diferencia de frameworks mais estruturados por buscar **menos papéis, menos níveis organizacionais e menos mecanismos adicionais de coordenação**.

Enquanto alguns modelos de escala introduzem estruturas específicas para portfólio, programas, planejamento e governança, o LeSS procura preservar ao máximo a simplicidade original do Scrum.

Isso não significa ausência de coordenação. Significa que a coordenação deve emergir principalmente da colaboração entre equipes, de um backlog compartilhado, de objetivos comuns e de transparência sobre o sistema como um todo.

## Fontes indicadas no material de referência

- LeSS — site oficial: https://less.works/
- Atlassian — Large-Scale Scrum (LeSS): https://www.atlassian.com/agile/agile-at-scale/less
- ProductPlan — LeSS (Large-Scale Scrum): https://www.productplan.com/glossary/less-large-scale-scrum
- Scrum Alliance — Large-Scale Scrum Certifications: https://www.scrumalliance.org/get-certified/large-scale-scrum-certifications


## Limites e cuidados de adoção

LeSS não é apenas uma agenda de eventos para coordenar muitos times. Sua aplicação pressupõe mudanças no desenho organizacional, equipes orientadas a funcionalidades, visão ampla de produto e redução de dependências e silos. Adotar apenas cerimônias, mantendo estruturas organizadas por componentes e múltiplas filas locais, tende a preservar justamente a complexidade que o framework procura reduzir.

Os intervalos de equipes são orientações empíricas do próprio LeSS, não limites matemáticos universais. O contexto do produto, a capacidade do Product Owner, a distribuição geográfica e a maturidade das equipes alteram a complexidade real.

## Páginas relacionadas

- [Nexus]({{ site.baseurl }}/Ágil-em-Escala/Nexus.html)
- [Gestão do Fluxo de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html)
- [Paralelo com SAFe]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Paralelo-com-SAFe.html)

## Proveniência e confiança

A síntese foi confrontada com a introdução e as regras oficiais do LeSS, incluindo a atualização de novembro de 2024.

**Confiança alta:** configurações Basic LeSS e LeSS Huge, produto e backlog compartilhados, Sprint comum e busca deliberada por menor complexidade organizacional.

**Confiança moderada:** resultados de uma adoção específica, pois dependem do contexto, do desenho organizacional e da qualidade da implementação.
