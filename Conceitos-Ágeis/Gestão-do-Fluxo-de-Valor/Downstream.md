---
title: "Downstream"
nav_order: 1
parent: "Gestão do Fluxo de Valor"
---

# Downstream

## O que é

Downstream é o subsistema do fluxo de valor em que trabalho já priorizado e suficientemente preparado é transformado em solução real, integrada, validada e entregue.

Se o upstream trabalha principalmente com **redução de incerteza**, o downstream trabalha principalmente com **execução sob compromisso**.

Ver [Gestão do Fluxo de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html) e [Upstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Upstream.html).

## O foco do downstream

O downstream deve otimizar a passagem de trabalho comprometido até a entrega de valor.

Fluxo ilustrativo:

```text
Trabalho pronto
      ↓
Planejamento / pull
      ↓
Construção
      ↓
Testes e validação
      ↓
Integração
      ↓
Deploy / disponibilização
      ↓
Entrega de valor
      ↓
Feedback e métricas
```

A sequência não precisa ser linear. Desenvolvimento, testes, integração e validação podem acontecer de forma sobreposta e contínua.

## Compromisso não significa rigidez

Entrar no downstream significa que a organização decidiu investir capacidade naquele trabalho. Isso não transforma escopo, solução ou plano em algo imutável.

Durante a execução podem surgir:

- aprendizado técnico;
- novas evidências de usuário;
- riscos não antecipados;
- mudanças de prioridade;
- necessidade de dividir o item;
- revisão de solução;
- descoberta de dependências.

A diferença importante é entre **aprendizado emergente**, que é inerente ao trabalho complexo, e **falta de entendimento mínimo**, que deveria ter sido tratada antes do compromisso.

## O downstream não é sinônimo de Sprint

Uma Sprint é apenas uma forma possível de organizar parte do downstream.

O downstream pode funcionar com:

- Scrum e iterações timeboxed;
- Kanban e fluxo contínuo;
- Scrumban;
- práticas DevOps e Continuous Delivery;
- combinações adequadas ao contexto.

O conceito descreve uma posição no fluxo de valor, não um framework específico.

## Qualidade faz parte do fluxo

Testes e qualidade não deveriam formar uma etapa tardia separada do desenvolvimento. Em um downstream saudável, qualidade é construída ao longo do fluxo.

Isso pode envolver:

- critérios de aceite claros;
- automação de testes;
- integração frequente;
- revisão de código;
- observabilidade;
- segurança incorporada ao desenvolvimento;
- validação contínua;
- Definition of Done adequada ao contexto.

Quanto mais tarde um problema é descoberto, maior tende a ser o custo de correção e maior o tempo de atravessamento do sistema.

## O papel do feedback

O downstream não termina simplesmente quando um item é "feito".

A entrega precisa gerar informação para o sistema:

```text
Entrega
  ↓
Uso / operação
  ↓
Métricas e feedback
  ↓
Aprendizado
  ↓
Nova decisão no upstream
```

Esse retorno permite revisar hipóteses, prioridades e soluções futuras. Sem ele, upstream e downstream tornam-se uma fábrica de output em vez de um sistema orientado a resultado.

## Sintomas de downstream sobrecarregado por upstream insuficiente

Alguns sinais recorrentes:

- histórias entram sem contexto de problema ou resultado esperado;
- o time precisa descobrir stakeholders básicos durante a implementação;
- dependências críticas aparecem no meio do ciclo;
- decisões de arquitetura são iniciadas tarde demais;
- dados ou acessos necessários ainda não existem;
- critérios de aceite são definidos depois que o desenvolvimento começou;
- grande quantidade de interrupções e retrabalho;
- itens retornam repetidamente para esclarecimento.

O diagnóstico útil não é simplesmente "o time precisa planejar melhor". A pergunta sistêmica é:

> **O trabalho foi puxado para o downstream antes de atingir maturidade suficiente?**

## Fluxo e previsibilidade

Um downstream saudável procura reduzir:

- filas;
- bloqueios;
- handoffs;
- lotes grandes;
- trabalho parcialmente concluído;
- retrabalho;
- dependências não geridas.

E aumentar:

- visibilidade do fluxo;
- qualidade embutida;
- frequência de integração;
- feedback;
- capacidade de entregar pequenos incrementos;
- previsibilidade baseada em dados do sistema.

Métricas de fluxo como lead time, cycle time, throughput, WIP e aging podem ajudar a entender o comportamento do downstream quando aplicáveis ao sistema adotado.

## Relação com o backlog mínimo

O backlog mínimo funciona como uma zona de readiness entre upstream e downstream. Seu objetivo é dar continuidade ao fluxo, não criar uma reserva rígida de meses de especificação pronta.

A quantidade saudável depende de fatores como:

- volatilidade de prioridades;
- duração do ciclo;
- velocidade de descoberta;
- dependências;
- risco técnico;
- capacidade e estabilidade do time.

Quanto mais volátil o contexto, maior tende a ser o desperdício causado por refinamento antecipado em excesso.

## Perguntas de diagnóstico

- Quanto tempo o trabalho leva entre compromisso e entrega?
- Onde os itens ficam bloqueados?
- Qual é o WIP real do time?
- Quanto retrabalho é causado por entendimento insuficiente?
- Testes e integração acontecem continuamente ou se acumulam no fim?
- O time entrega incrementos pequenos ou grandes lotes?
- A conclusão técnica gera feedback de uso e resultado?
- Esse feedback efetivamente retorna ao upstream?

## Páginas relacionadas

- [Gestão do Fluxo de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html)
- [Upstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Upstream.html)
- [Fluxo End to End]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Fluxo-End-to-End.html)
- [Release, Deploy e Entrega de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Release-Deploy-e-Entrega-de-Valor.html)
- [Paralelo com SAFe]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Paralelo-com-SAFe.html)

## Fontes

- Ver [Gestão do Fluxo de Valor — Fontes e proveniência]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html#fontes-e-proveniência).
