---
title: "Upstream"
nav_order: 4
parent: "Gestão do Fluxo de Valor"
---

# Upstream

## O que é

Upstream é o subsistema do fluxo de valor voltado a **reduzir incerteza antes do compromisso de execução**. Ele transforma necessidades, problemas, oportunidades e ideias em trabalho suficientemente compreendido, priorizado e preparado para ser puxado pelo [Downstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Downstream.html).

O upstream é a fase inicial desse fluxo, onde ocorrem atividades essenciais de planejamento, estratégia e definição de direção.

Nas metodologias ágeis, o upstream é onde as bases são estabelecidas – é onde a equipe define os objetivos do projeto, estabelece requisitos claros e cria uma visão geral do trabalho a ser realizado. Em essência, o upstream é a raiz do sucesso de um projeto ágil.

A pergunta dominante não é apenas "como construir?", mas principalmente:

> **Qual problema merece atenção, por que agora e o que precisamos aprender antes de comprometer capacidade?**

Ver [Gestão do Fluxo de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html).

## Diferença entre Upstream e Downstream

Para entender plenamente o upstream, é importante distinguir os termos **upstream** e **downstream**.

O [Downstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Downstream.html) é a fase subsequente do fluxo de trabalho, onde ocorrem a execução, os testes, a integração e a entrega. Enquanto o downstream se concentra na implementação do que foi planejado e suficientemente definido no upstream, o upstream está focado em preparar o terreno para que a execução aconteça com maior clareza, menor incerteza e melhores condições de fluxo.

Em termos simples:

```text
UPSTREAM
Entender → Priorizar → Descobrir → Refinar → Preparar

                         ↓ ponto de compromisso

DOWNSTREAM
Planejar → Construir → Testar → Integrar → Entregar
```

A diferença central está no tipo de problema que cada sistema procura resolver:

- **Upstream:** reduz incerteza e prepara decisões e trabalho futuro.
- **Downstream:** transforma trabalho preparado em incremento e valor entregue.

Essa distinção é importante para manter clareza sobre as atividades e responsabilidades ao longo do fluxo, criar entendimento comum sobre os objetivos e evitar que o time de execução precise absorver continuamente decisões, descobertas e definições que poderiam ter sido tratadas antes do ponto de compromisso.

Isso não significa que upstream e downstream funcionem de forma isolada ou estritamente sequencial. Em um fluxo saudável, ambos operam de maneira contínua e conectada: enquanto o downstream executa e gera feedback, o upstream prepara e ajusta os próximos itens com base no aprendizado produzido pela própria entrega.

## Três horizontes do upstream

### 1. Estratégico

Objetivo: selecionar problemas, oportunidades e iniciativas coerentes com a direção da organização.

Perguntas típicas:

- Qual objetivo estratégico queremos mover?
- Que necessidade ou oportunidade merece investimento?
- Qual resultado esperamos alcançar?
- Quais iniciativas competem pela mesma capacidade?
- Qual risco existe em fazer, não fazer ou adiar?

Objetos comuns:

- visão e objetivos;
- necessidades e oportunidades;
- ideias e hipóteses;
- indicadores e resultados esperados;
- iniciativas;
- prioridades e riscos.

Fluxo ilustrativo:

```text
Visão / objetivos
       ↓
Necessidades / ideias
       ↓
Priorização
       ↓
Descoberta
```

Neste horizonte, o objeto de trabalho normalmente ainda é maior que uma história de usuário. Pode ser uma iniciativa, hipótese, épico, problema ou oportunidade.

### 2. Tático

Objetivo: transformar uma iniciativa priorizada em algo executável sem tentar especificá-la por completo.

Perguntas típicas:

- O problema está suficientemente compreendido?
- Qual é o menor recorte coerente de valor?
- Como o usuário ou processo é afetado?
- Quais capacidades ou funcionalidades serão necessárias?
- Existem restrições técnicas, de dados, segurança, infraestrutura ou compliance?
- Quais dependências podem bloquear a execução?
- Como saberemos se a solução atende ao que foi proposto?

Práticas e artefatos possíveis:

- jornadas e story mapping;
- processos AS IS / TO BE;
- MVP e recortes incrementais;
- épicos, features, histórias e enablers;
- critérios de aceite;
- desenho de solução;
- arquitetura;
- estratégia de testes;
- análise de dados, segurança e infraestrutura;
- dependências;
- estimativas.

O princípio central é **maturação conjunta entre negócio, produto e tecnologia**.

### 3. Readiness e ponto de compromisso

Objetivo: decidir se existe informação suficiente para puxar o item para execução.

```text
Exploração
   ↓
Refinamento de negócio
   ↓
Refinamento técnico
   ↓
Estimativa / capacidade
   ↓
Readiness
   ↓
Ponto de compromisso
   ↓
Downstream
```

A política de readiness pode considerar:

- valor ou resultado esperado claro;
- prioridade explícita;
- escopo inicial compreensível;
- critérios de aceite proporcionais ao risco;
- dependências críticas conhecidas;
- principais riscos técnicos tratados ou visíveis;
- tamanho suficiente para planejamento;
- capacidade disponível;
- estratégia mínima de validação.

**Readiness não significa certeza.** Significa apenas que a incerteza residual é aceitável para assumir compromisso.

## Backlog mínimo: upstream, downstream ou fronteira?

Em modelos organizacionais diferentes, a formação de um backlog mínimo pode aparecer no fim do upstream ou no início operacional do downstream. Por isso, nesta base ele é tratado como uma **zona de transição**.

O ponto importante não é classificar a caixa no diagrama, e sim garantir que exista uma quantidade saudável de trabalho pronto para sustentar o fluxo.

```text
Insuficiente
→ espera ou improvisação no downstream

Excessivo
→ refinamento antecipado
→ itens envelhecem
→ prioridade pode mudar

Saudável
→ continuidade sem estoque desnecessário
```

Não existe uma quantidade universal de semanas ou meses que defina um backlog mínimo correto.

## Upstream não é um funil de aprovação

O upstream deve favorecer decisão rápida e redução progressiva de incerteza. Ele perde valor quando vira uma sequência rígida de handoffs e aprovações.

### Anti-padrão: mini-Waterfall

```text
Ideia
→ análise completa
→ requisitos completos
→ arquitetura completa
→ aprovação completa
→ somente então desenvolvimento
```

### Fluxo adaptativo

```text
Identificar a maior incerteza
→ aprender o suficiente
→ reduzir lote
→ comprometer
→ entregar
→ medir
→ retroalimentar o upstream
```

A pergunta correta não é "está tudo definido?", e sim:

> **Sabemos o suficiente para começar este próximo incremento com risco aceitável?**

## Refinamento contínuo e WIP

O upstream também precisa de gestão de fluxo. Se muitas iniciativas forem exploradas simultaneamente, a organização cria um grande estoque de trabalho parcialmente analisado.

Boas práticas incluem:

- limitar trabalho em exploração;
- explicitar estados e critérios de passagem;
- descartar hipóteses sem valor antes de refiná-las demais;
- priorizar por valor, risco, urgência e capacidade;
- evitar refinamento detalhado muito antes da execução;
- medir tempo de espera e envelhecimento dos itens;
- tratar dependências cedo, mas apenas no nível necessário.

Backlog refinado em excesso pode ser entendido como **WIP futuro**: trabalho que já consumiu capacidade, mas ainda não produziu valor.

## Relação com Discovery

Product Discovery está contido no upstream, mas não cobre necessariamente todo o upstream organizacional. O upstream pode começar antes do time de produto, na formulação e priorização de iniciativas, e continuar até a definição da política de entrada no sistema de execução.

## Relação com Scrum

O refinamento do Product Backlog contribui para o upstream próximo ao time, mas não representa sozinho todo o sistema. Estratégia, priorização entre iniciativas, descoberta e coordenação de dependências podem ocorrer em níveis organizacionais acima de um Scrum Team.

## Relação com Kanban

Kanban pode ser usado diretamente no upstream para visualizar estados de descoberta e análise, limitar WIP e tornar explícitas as políticas de compromisso. O mesmo pensamento pode continuar no downstream, formando um fluxo integrado.

## Perguntas de diagnóstico

- Quantos itens estão sendo refinados sem perspectiva real de execução?
- Quanto tempo uma ideia leva para chegar ao ponto de compromisso?
- Onde as iniciativas ficam esperando?
- Que informação realmente reduz risco e que documentação existe apenas por hábito?
- Quais dependências são descobertas tarde demais?
- O time está recebendo problemas bem contextualizados ou apenas soluções prescritas?
- O feedback de entregas anteriores está alterando as prioridades atuais?

## Páginas relacionadas

- [Gestão do Fluxo de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html)
- [Downstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Downstream.html)
- [Fluxo End to End]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Fluxo-End-to-End.html)
- [Paralelo com SAFe]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Paralelo-com-SAFe.html)

## Fontes

- Ver [Gestão do Fluxo de Valor — Fontes e proveniência]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html#fontes-e-proveniência).