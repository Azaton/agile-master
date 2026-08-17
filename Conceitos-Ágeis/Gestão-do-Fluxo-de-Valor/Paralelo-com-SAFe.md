---
title: "Paralelo com SAFe"
nav_order: 3
parent: "Gestão do Fluxo de Valor"
---

Esta página compara o modelo conceitual de [Upstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Upstream.html)/[Downstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Downstream.html) com elementos do **SAFe (Scaled Agile Framework)**.

O paralelo é útil porque os dois procuram conectar estratégia e execução em escala, mas **não existe equivalência formal termo a termo**.

- upstream/downstream é uma lente de fluxo;
- SAFe é um framework estruturado de organização e entrega em escala.

Ver [Gestão do Fluxo de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html). Para uma introdução ao framework em si, ver [SAFe]({{ site.baseurl }}/Ágil-em-Escala/SAFe.html), em Ágil em Escala.

## O problema sistêmico em comum

Ambos ajudam a responder uma pergunta parecida:

> **Como transformar estratégia e necessidades em trabalho executável pelos times, preservando prioridade, alinhamento, arquitetura, dependências, capacidade e feedback?**

O modelo upstream/downstream responde organizando o sistema em torno de **redução de incerteza → compromisso → execução → feedback**.

SAFe distribui responsabilidades e mecanismos por elementos como portfólio, Agile Release Trains (ARTs), backlogs, Continuous Delivery Pipeline e eventos de inspeção e adaptação.

## Correspondências úteis — sem equivalência rígida

| Gestão de fluxo | Elementos do SAFe que se aproximam |
|---|---|
| Estratégia e objetivos | Strategic Themes / Portfolio Vision |
| Ideias e iniciativas | Portfolio Epics / Portfolio Backlog |
| Priorização | Portfolio Kanban / mecanismos econômicos de priorização como WSJF, quando aplicável |
| Descoberta | Continuous Exploration / análise de Epics / Product Management |
| Refinamento de negócio | Features, Stories e refinamento de backlog |
| Refinamento técnico | Enablers, arquitetura e práticas de Agile Product Delivery |
| Readiness | Features priorizadas no ART Backlog e Stories refinadas no Team Backlog |
| Ponto de compromisso | decisões de planejamento e pull de trabalho em ARTs e times |
| Construção e validação | Continuous Integration |
| Disponibilização técnica | Continuous Deployment |
| Entrega ao usuário/mercado | Release on Demand |
| Feedback | métricas de solução, Release on Demand, Inspect & Adapt e nova Continuous Exploration |

A tabela é deliberadamente aproximada. Um mesmo elemento SAFe pode participar de mais de uma parte do fluxo, e a fronteira upstream/downstream depende da política concreta de cada sistema.

## Portfolio Kanban como exemplo de upstream organizacional

O **Portfolio Kanban** é um dos pontos de contato mais claros.

No SAFe, ele ajuda a tornar visível o fluxo de Epics entre estados de entrada, análise, readiness, implementação e conclusão. Isso se aproxima do upstream organizacional porque coloca atenção explícita em:

- seleção de iniciativas;
- análise antes do compromisso;
- limites de WIP;
- alinhamento estratégico;
- decisão econômica;
- governança do fluxo de Epics.

Essa associação é especialmente relevante porque mostra que upstream não precisa ser tratado como uma sequência de reuniões ou documentos. Ele pode ser gerido como **sistema Kanban com políticas, WIP e decisões de fluxo**.

## Continuous Exploration e upstream

No SAFe, **Continuous Exploration (CE)** é a primeira parte do Continuous Delivery Pipeline. Ela trabalha continuamente mercado e necessidades de clientes, visão, roadmap e Features priorizadas para o ART Backlog.

Conceitualmente:

```text
Continuous Exploration
≈ forte componente de upstream
```

A aproximação é alta porque CE também busca decidir e preparar **o que deve ser construído** antes de a funcionalidade avançar pelo restante do pipeline.

Mesmo assim, upstream pode começar antes da CE quando a lente utilizada inclui estratégia corporativa, portfólio e seleção de iniciativas.

## Continuous Integration, Continuous Deployment e downstream

O SAFe define o Continuous Delivery Pipeline com quatro partes:

1. Continuous Exploration;
2. Continuous Integration;
3. Continuous Deployment;
4. Release on Demand.

As três últimas se aproximam fortemente do downstream:

```text
Continuous Integration
→ desenvolver, testar, integrar e validar

Continuous Deployment
→ mover funcionalidade validada para produção

Release on Demand
→ disponibilizar valor de acordo com necessidade de negócio e clientes
```

Assim, uma leitura didática possível é:

```text
                 CONTINUOUS DELIVERY PIPELINE

UPSTREAM                         DOWNSTREAM
────────                         ──────────
Continuous Exploration   →   Continuous Integration
                              ↓
                         Continuous Deployment
                              ↓
                         Release on Demand
                              ↓
                            Feedback
                              └────→ Continuous Exploration
```

Essa representação ajuda a perceber que o próprio pipeline do SAFe é descrito como um **ciclo contínuo de aprendizado e entrega**, não como uma cadeia linear de fases.

## Portfolio, ART e Team: escalas diferentes do mesmo fluxo

Uma diferença importante é que o SAFe explicita múltiplas escalas de decisão.

### Portfolio

Preocupações predominantes:

- estratégia;
- investimentos;
- Epics;
- prioridades;
- value streams;
- alinhamento entre estratégia e execução.

Tem forte concentração de atividades de upstream.

### ART

Preocupações predominantes:

- Features;
- arquitetura;
- dependências;
- planejamento integrado;
- integração da solução;
- entrega de valor.

O ART atravessa a fronteira: participa tanto da preparação quanto da execução.

### Team

Preocupações predominantes:

- Stories e Enablers;
- refinamento próximo da implementação;
- planejamento e execução;
- qualidade;
- integração e feedback.

O time também possui upstream local. Portanto, seria incorreto dizer que "Portfolio é upstream e Team é downstream" de forma absoluta.

O padrão mais preciso é **upstreams e downstreams aninhados em diferentes escalas**.

## Inspect & Adapt e o fechamento do ciclo

O evento **Inspect & Adapt (I&A)** reforça outro ponto importante: execução não termina no output.

No SAFe, o I&A cria um ciclo de inspeção da solução, medição e identificação estruturada de melhorias no ART. Os itens de melhoria retornam ao backlog e influenciam ciclos futuros.

Isso se alinha diretamente com a ideia desta base:

```text
Downstream
→ resultado e evidência
→ feedback
→ mudança no upstream
```

## Onde o paralelo deixa de funcionar

Existem diferenças importantes:

- SAFe define estruturas, papéis, eventos, backlogs e competências próprias;
- upstream/downstream pode ser usado sem ART, PI, Epic ou qualquer terminologia SAFe;
- SAFe trata explicitamente portfólio, desenvolvimento de produto, arquitetura, DevOps e coordenação em escala;
- upstream/downstream é uma abstração mais leve para enxergar fluxo e compromisso;
- uma implementação de SAFe pode ter múltiplos pontos de upstream/downstream em níveis diferentes.

Por isso, o modelo não deve ser descrito como "um SAFe simplificado".

## Uma leitura em camadas

Uma forma útil de combinar as duas lentes é:

```text
ESTRATÉGIA / PORTFÓLIO
        ↓
 upstream organizacional
        ↓
ART / coordenação de solução
        ↓
 upstream próximo da execução
        ↓
 ponto de compromisso
        ↓
 times / downstream
        ↓
 integração / deploy / release
        ↓
 feedback
        └────────────→ estratégia e exploração
```

Isso preserva a principal contribuição de upstream/downstream: olhar para o fluxo completo sem confundir cada etapa com uma estrutura formal específica.

## Relação futura com Flight Levels

Flight Levels é um estudo complementar importante porque também separa preocupações de estratégia, coordenação e operação. Ele pode oferecer uma segunda lente organizacional para comparar com este conteúdo, sem pressupor a adoção de SAFe.

## Páginas relacionadas

- [Gestão do Fluxo de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html)
- [Upstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Upstream.html)
- [Downstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Downstream.html)
- [Fluxo End to End]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Fluxo-End-to-End.html)

## Referências oficiais do SAFe

- Scaled Agile Framework — Strategic Themes: https://framework.scaledagile.com/strategic-themes
- Scaled Agile Framework — Portfolio Backlog / Portfolio Kanban: https://framework.scaledagile.com/portfolio-backlog
- Scaled Agile Framework — Continuous Delivery Pipeline: https://framework.scaledagile.com/continuous-delivery-pipeline
- Scaled Agile Framework — Continuous Exploration: https://framework.scaledagile.com/continuous-exploration
- Scaled Agile Framework — Continuous Integration: https://framework.scaledagile.com/continuous-integration
- Scaled Agile Framework — Continuous Deployment: https://framework.scaledagile.com/continuous-deployment
- Scaled Agile Framework — Release on Demand: https://framework.scaledagile.com/release-on-demand
- Scaled Agile Framework — Team Backlog: https://framework.scaledagile.com/team-backlog
- Scaled Agile Framework — Inspect & Adapt: https://framework.scaledagile.com/inspect-and-adapt
