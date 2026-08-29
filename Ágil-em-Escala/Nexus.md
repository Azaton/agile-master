---
title: "Nexus"
nav_order: 2
parent: "Ágil em Escala"
---

# Nexus Framework

## O que é

**Nexus** é um framework criado para **escalar Scrum quando múltiplos Scrum Teams trabalham juntos sobre um único produto**.

Ele foi desenvolvido por **Ken Schwaber e Scrum.org** e publicado originalmente em 2015. A proposta central é preservar Scrum e adicionar somente os elementos estritamente necessários para lidar com os problemas que aparecem quando vários times precisam colaborar sobre o mesmo produto, principalmente **dependências entre equipes, integração e coordenação do trabalho**.

Um Nexus reúne aproximadamente **3 a 9 Scrum Teams** trabalhando de forma coordenada sobre:

- **um único produto**;
- **um único Product Owner**;
- **um único Product Backlog**;
- **um Product Goal compartilhado**;
- **um Integrated Increment** ao final de cada Sprint.

A ideia central pode ser resumida assim:

> **Scaled Scrum is still Scrum.**

Ou seja: escalar Scrum não significa substituir Scrum por uma estrutura organizacional inteiramente nova. Nexus procura manter a base do framework original e expandi-la apenas onde a escala gera novas necessidades.

## O problema que o Nexus busca resolver

Quando vários Scrum Teams trabalham no mesmo produto, cresce a quantidade de relações entre pessoas, componentes, decisões e entregas.

Com isso, surgem problemas como:

- dependências entre equipes;
- trabalho que só pode ser concluído depois do trabalho de outro time;
- conflitos de integração;
- incremento parcial ou incompatível entre equipes;
- dificuldade de visualizar o estado real do produto;
- decisões locais que prejudicam o produto como um todo;
- aumento dos caminhos de comunicação e coordenação.

Nexus procura tornar essas dependências e problemas de integração **transparentes, reduzidos ou eliminados sempre que possível**.

O objetivo não é simplesmente coordenar mais pessoas. É permitir que vários Scrum Teams entreguem juntos **mais valor do que conseguiriam trabalhando como grupos isolados**.

## Estrutura conceitual

Uma representação simplificada é:

```text
                       Produto
                          ↓
                    Product Owner
                          ↓
                  Product Backlog
                          ↓
          ┌───────────────┼───────────────┐
          ↓               ↓               ↓
    Scrum Team A     Scrum Team B     Scrum Team C
          └───────────────┼───────────────┘
                          ↓
               Trabalho integrado
                          ↓
               Integrated Increment
```

Todas as equipes trabalham sobre o mesmo produto e contribuem para **um único incremento integrado**, em vez de gerar incrementos independentes que só seriam integrados posteriormente.

## Nexus Integration Team

A principal accountability adicional criada pelo Nexus é o **Nexus Integration Team (NIT)**.

Sua responsabilidade é garantir que o Nexus produza, pelo menos uma vez por Sprint, um **Integrated Increment valioso e utilizável**.

O Nexus Integration Team é composto por:

- o **Product Owner**;
- um **Scrum Master**;
- **Nexus Integration Team Members**, conforme necessário.

O NIT não substitui os Scrum Teams nem funciona como uma equipe de controle central sobre eles.

Seu foco está nos problemas que atravessam os limites de um único time, especialmente:

- integração;
- dependências;
- transparência do incremento;
- impedimentos que afetam múltiplas equipes;
- melhoria da capacidade do Nexus de entregar como um sistema único.

Uma ideia importante do framework é que problemas que afetam múltiplos times precisam ganhar prioridade suficiente para não serem tratados apenas como responsabilidade local de uma das equipes.

## Eventos do Nexus

Nexus preserva a Sprint e amplia alguns eventos do Scrum para trabalhar na escala de múltiplas equipes.

### Sprint

A Sprint em Nexus mantém o mesmo significado existente em Scrum.

Durante a Sprint, os Scrum Teams trabalham de forma coordenada para produzir **um único Integrated Increment**.

### Cross-Team Refinement

O **Cross-Team Refinement** tem como foco identificar e reduzir dependências entre equipes antes que elas prejudiquem a execução.

Durante o refinamento, o Product Backlog deve ser compreendido em um nível suficiente para que:

- dependências entre itens sejam identificadas;
- dependências entre equipes fiquem transparentes;
- o trabalho possa ser reorganizado ou decomposto;
- dependências possam ser removidas ou minimizadas.

Esse é um dos pontos mais característicos do Nexus: não basta refinar o conteúdo funcional; é necessário refinar também **a estrutura das dependências entre os times**.

### Nexus Sprint Planning

O **Nexus Sprint Planning** coordena o planejamento da Sprint no nível do Nexus.

O resultado inclui:

- um **Nexus Sprint Goal**, alinhado ao Product Goal;
- um Sprint Goal para cada Scrum Team, alinhado ao objetivo do Nexus;
- um **Nexus Sprint Backlog**;
- Sprint Backlogs de cada equipe.

O Nexus Sprint Backlog torna transparente o trabalho necessário para alcançar o Nexus Sprint Goal e, principalmente, as dependências existentes entre as equipes.

### Nexus Daily Scrum

O **Nexus Daily Scrum** é voltado à inspeção do progresso do Nexus em direção ao Nexus Sprint Goal.

Seu foco está especialmente em questões que atravessam as equipes:

- novas dependências;
- problemas de integração;
- impedimentos entre times;
- necessidade de coordenação durante a Sprint.

Ele não elimina a Daily Scrum de cada equipe.

### Nexus Sprint Review

A **Nexus Sprint Review** inspeciona o **Integrated Increment** produzido pelo Nexus como um todo.

O foco deixa de ser analisar entregas isoladas por equipe e passa a ser avaliar o estado real do produto integrado e obter feedback dos stakeholders.

### Nexus Sprint Retrospective

A **Nexus Sprint Retrospective** busca melhorar a forma como todo o Nexus trabalha.

Além dos problemas internos de cada equipe, deve permitir a inspeção de fatores sistêmicos como:

- dependências recorrentes;
- problemas de integração;
- estrutura do produto;
- fluxo de trabalho entre equipes;
- comunicação;
- práticas de desenvolvimento;
- impedimentos organizacionais.

## Artefatos e compromissos

### Product Backlog

Existe **um único Product Backlog** para todo o Nexus.

Todos os Scrum Teams trabalham a partir dele.

O Product Owner continua responsável pelo conteúdo, disponibilidade e ordenação do backlog.

**Compromisso associado:** Product Goal.

### Nexus Sprint Backlog

O **Nexus Sprint Backlog** fornece transparência sobre o trabalho que o Nexus precisa realizar durante a Sprint para atingir o Nexus Sprint Goal.

Ele ajuda a visualizar especialmente **dependências entre equipes**.

**Compromisso associado:** Nexus Sprint Goal.

### Integrated Increment

O **Integrated Increment** representa a soma de todo o trabalho integrado e concluído pelos Scrum Teams durante a Sprint.

Não é uma simples coleção de incrementos independentes. O resultado precisa funcionar como um **produto integrado**.

**Compromisso associado:** Definition of Done.

## A importância da integração contínua

A palavra central do Nexus é **integração**.

Quando existem vários times, deixar a integração para o final da Sprint ou para uma fase posterior cria grande risco.

Um padrão problemático seria:

```text
Equipe A → entrega parte A
Equipe B → entrega parte B
Equipe C → entrega parte C

                 ↓
          integração tardia
                 ↓
           muitos conflitos
```

Nexus procura favorecer outro comportamento:

```text
Equipe A ─┐
Equipe B ─┼── integração contínua ──→ Integrated Increment
Equipe C ─┘
```

Quanto mais cedo os times integrarem trabalho, mais cedo problemas de dependência e compatibilidade se tornam visíveis.

## Dependências são o principal problema de escala

Uma ideia fundamental do Nexus é que aumentar o número de pessoas não aumenta valor automaticamente.

Adicionar equipes também aumenta:

- complexidade;
- dependências;
- caminhos de comunicação;
- necessidade de colaboração;
- esforço de integração.

Por isso, o framework enfatiza que **reduzir o número de pessoas ou equipes envolvidas em determinado trabalho também pode ser uma estratégia válida de escala**.

Escalar não significa necessariamente tornar a estrutura maior. Pode significar tornar o sistema mais simples e reduzir dependências.

## Nexus e Scrum tradicional

A lógica básica pode ser comparada desta forma:

```text
SCRUM

1 Product Owner
1 Product Backlog
1 Scrum Team
1 Sprint
1 Incremento
```

```text
NEXUS

1 Product Owner
1 Product Backlog
3–9 Scrum Teams
1 Sprint compartilhada
1 Nexus Sprint Goal
1 Integrated Increment
```

Nexus mantém os princípios centrais de Scrum e adiciona mecanismos para tratar aquilo que passa a existir quando vários times compartilham o mesmo produto.

## Nexus e LeSS

Nexus e [LeSS]({{ site.baseurl }}/Ágil-em-Escala/LeSS.html) têm uma característica estrutural importante em comum:

- múltiplos times;
- um único produto;
- um único Product Owner;
- um único Product Backlog;
- foco em um incremento integrado.

A diferença principal está na forma como os dois frameworks tratam a coordenação em escala.

**LeSS** procura manter a estrutura organizacional extremamente simples e minimizar mecanismos adicionais de coordenação.

**Nexus** também preserva Scrum, mas formaliza alguns elementos adicionais especificamente para tratar dependências e integração, como:

- Nexus Integration Team;
- Cross-Team Refinement;
- Nexus Sprint Planning;
- Nexus Daily Scrum;
- Nexus Sprint Backlog;
- Nexus Sprint Goal.

Assim, os dois frameworks partem de uma filosofia semelhante — **escalar Scrum sem transformar o processo em uma estrutura excessivamente burocrática** —, mas Nexus torna a coordenação entre equipes um pouco mais explícita.

## Quando Nexus faz sentido

Nexus é particularmente aplicável quando:

- existe **um único produto**;
- múltiplos Scrum Teams trabalham nesse produto;
- existem dependências entre as equipes;
- essas dependências dificultam sincronização e integração;
- a organização quer continuar usando Scrum como fundamento do trabalho.

Se as equipes trabalham sobre produtos independentes e praticamente não possuem dependências entre si, talvez não exista a necessidade de tratá-las como um Nexus.

## Princípios que merecem destaque

### Scrum escalado continua sendo Scrum

Nexus não pretende substituir Scrum.

A lógica é preservar empirismo, transparência, inspeção, adaptação e os Scrum Values enquanto se trata a complexidade adicional causada pela escala.

### Um produto, não vários projetos de equipe

As equipes devem olhar para um **produto compartilhado**.

O sucesso do Nexus não é a soma de vários times "cumprindo sua parte", mas a entrega de um produto integrado que gere valor.

### Transparência das dependências

Dependências escondidas criam atrasos e integração tardia.

Nexus procura torná-las visíveis cedo para que possam ser reduzidas ou eliminadas.

### Integração é responsabilidade do sistema

A integração não deve ser delegada para uma fase final nem para uma equipe isolada.

Todo o Nexus precisa trabalhar de forma que um incremento integrado exista pelo menos uma vez em cada Sprint.

## Fonte principal

Este conteúdo foi construído principalmente a partir das referências oficiais da Scrum.org:

- Nexus Framework for Scaling Scrum: https://www.scrum.org/resources/nexus-framework-scaling-scrum
- Nexus Guide: https://www.scrum.org/resources/nexus-guide
- Online Nexus Guide: https://www.scrum.org/resources/online-nexus-guide
- Scaling Scrum with Nexus: https://www.scrum.org/resources/scaling-scrum

A versão do Nexus Guide utilizada como referência conceitual é a edição de **janeiro de 2021**.

## Limites e cuidados de adoção

Nexus não elimina dependências por meio de mais reuniões. Seus eventos e artefatos tornam problemas de integração visíveis, mas a organização ainda precisa investir em arquitetura, integração contínua, equipes capazes de entregar valor e redução efetiva das dependências.

O intervalo de aproximadamente três a nove Scrum Teams descreve o campo de aplicação apresentado pela Scrum.org. Não deve ser interpretado como garantia de que qualquer conjunto de equipes nessa faixa formará um Nexus saudável.

## Páginas relacionadas

- [LeSS]({{ site.baseurl }}/Ágil-em-Escala/LeSS.html)
- [Gestão do Fluxo de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html)

## Proveniência e confiança

A página foi construída a partir do Nexus Guide e dos materiais oficiais da Scrum.org. A edição de janeiro de 2021 permanece como referência conceitual indicada na fonte original desta curadoria.

**Confiança alta:** finalidade do Nexus, faixa aproximada de equipes, Integrated Increment, Nexus Integration Team, eventos e artefatos.

**Confiança moderada:** adequação do framework a uma organização específica, que depende do produto, das dependências e da capacidade técnica de integração.
