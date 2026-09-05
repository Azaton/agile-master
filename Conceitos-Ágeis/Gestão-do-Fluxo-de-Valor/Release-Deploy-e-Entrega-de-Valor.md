---
title: "Release, Deploy e Entrega de Valor"
nav_order: 5
parent: "Gestão do Fluxo de Valor"
---

# Release, Deploy e Entrega de Valor

## Em resumo

- **Commit, Pull Request, merge, tag, release e deployment são eventos diferentes.** Nenhum deles comprova isoladamente que uma mudança chegou aos usuários ou produziu valor.
- **Uma release combina identidade técnica e referências temporais.** Ela pode ter versão, tag ou commit de referência, data de corte, publicação e deployments em datas distintas.
- **Uma janela gerencial não substitui uma versão técnica.** Quando vários deployments são consolidados em um período, é preciso explicitar o que foi incluído, onde foi implantado e quando ficou disponível.
- **Sprint não é release.** Um Incremento Done pode ser liberado antes do fim da Sprint, e a Sprint Review não deve funcionar como barreira para liberar valor.
- **A boa governança conecta tecnologia, produto e gestão.** Uma release confiável permite responder o que mudou, qual versão representa a mudança, onde está disponível e quais resultados foram observados.

## O que é

Uma **release** é uma versão identificável de um produto ou software preparada para disponibilização. Ela reúne mudanças selecionadas e deve permitir compreender o que mudou, qual estado técnico representa e como se relaciona com os ambientes em que foi implantada.

Em plataformas como o GitHub, a release normalmente se apoia em uma tag que aponta para um ponto específico do histórico. No contexto organizacional, o mesmo termo também pode designar a janela usada para planejar e comunicar um conjunto de entregas. Esta página conecta esses dois sentidos sem tratá-los como equivalentes.

## O problema de linguagem

Em conversas entre gestão, produto e desenvolvimento, a palavra **release** pode assumir sentidos diferentes.

Para a gestão, uma release frequentemente representa um pacote de entregas consolidado e comunicado dentro de uma janela de tempo. Para desenvolvimento, ela tende a representar uma versão identificável e reproduzível do software. As duas perspectivas podem ser legítimas, mas descrevem dimensões diferentes.

O problema começa quando termos distintos passam a ser tratados como sinônimos:

- commit não é Pull Request;
- Pull Request não é merge;
- merge não é release;
- release não é necessariamente deployment;
- deployment não comprova, sozinho, entrega de valor.

Uma linguagem comum melhora a rastreabilidade e evita que uma mesma frase — como “isso entrou na release” — seja interpretada de maneiras incompatíveis.

## A distinção central

> **Uma release não é definida apenas por uma data, mas também não existe completamente fora do tempo.**

Uma release possui uma identidade, um conteúdo e um ponto de referência. Ao mesmo tempo, seu ciclo produz eventos temporais: definição da janela, data de corte, criação da tag, publicação, deployments e disponibilização aos usuários.

Por isso, dizer que “release não tem data” é impreciso. O que pode não existir é uma data embutida no **nome ou número da versão**.

Da mesma forma, dizer que “tudo que teve commit durante o período pertence automaticamente à release” também é impreciso. A inclusão depende do estado do código, da estratégia de branches, da tag adotada, de reversões, feature flags e do processo de implantação.

## Vocabulário compartilhado

| Elemento | O que representa | O que não garante |
|---|---|---|
| **Commit** | Um ponto registrado no histórico do código, contendo um estado do projeto | Que a mudança foi revisada, integrada ou implantada |
| **Pull Request (PR)** | Uma proposta para discutir, revisar e integrar mudanças entre branches | Que as mudanças foram aprovadas, mescladas ou publicadas |
| **Merge** | A incorporação de históricos ou mudanças em uma branch de destino | Que o conteúdo chegou à produção |
| **Tag** | Uma referência nominal para um ponto específico do histórico | Que exista uma release publicada ou um deployment |
| **Release** | Uma versão identificável do produto, associada a mudanças selecionadas | Que a versão esteja disponível em todos os ambientes |
| **Deployment** | A implantação de uma versão em um ambiente | Que usuários já tenham acesso ou que valor tenha sido produzido |
| **Entrega de valor** | Uma capacidade utilizável que produz resultado ou aprendizado | Que o resultado esperado tenha sido alcançado |

O Git trata commits como pontos do histórico e snapshots relacionados do conteúdo do projeto. No GitHub, Pull Requests são propostas de integração que concentram discussão, revisão, verificações e mudanças antes do merge.

## Da mudança ao aprendizado

```text
Necessidade priorizada
        ↓
Construção
        ↓
Commit
        ↓
Pull Request e revisão
        ↓
Merge e integração
        ↓
Tag / versão de referência
        ↓
Release
        ↓
Deployment por ambiente
        ↓
Disponibilização aos usuários
        ↓
Uso, resultado e feedback
```

Esse fluxo é ilustrativo, não uma prescrição universal. Organizações podem automatizar etapas, publicar releases antes do deployment, implantar antes de liberar uma funcionalidade ou operar com estratégias diferentes de branches e versionamento.

O ponto essencial é que **o histórico do repositório, a versão publicada, a implantação técnica e o valor em uso são evidências diferentes**.

## Dois sentidos que precisam ser explicitados

### 1. Release técnica

É uma versão identificável e, idealmente, reproduzível do produto. Em um repositório Git, costuma ser vinculada a uma tag ou a um commit de referência.

No GitHub, uma release é baseada em uma tag que marca um ponto específico no histórico. A plataforma também registra sua publicação e permite associar notas e artefatos.

Perguntas típicas:

- Qual tag ou commit representa a versão?
- Quais artefatos foram gerados?
- Quais mudanças foram incluídas?
- É possível reconstruir ou restaurar essa versão?
- Em quais ambientes ela foi implantada?

### 2. Release gerencial ou janela de entrega

É um agrupamento usado para planejar, consolidar e comunicar mudanças produzidas durante determinado intervalo.

Perguntas típicas:

- Qual objetivo essa entrega atende?
- Qual período foi considerado?
- Quais funcionalidades e correções estão sendo comunicadas?
- O que ficou de fora?
- Quais riscos e pendências permanecem?
- O que está efetivamente disponível aos usuários?

A janela de entrega é uma convenção de governança. Ela não substitui a referência técnica da versão.

Quando uma “release” reúne retrospectivamente vários deployments ocorridos durante meses, o termo mais preciso pode ser **relatório consolidado de entregas do período**. Se a organização optar por manter o nome release, deve deixar explícito que se trata de uma consolidação gerencial, e não de um único evento técnico de implantação.

## Afinal, quais datas uma release pode ter?

| Referência temporal | O que informa |
|---|---|
| **Início da janela** | Desde quando as mudanças estão sendo consideradas |
| **Data de corte** | Limite definido para entrada de mudanças no pacote |
| **Criação da tag** | Quando o estado técnico recebeu uma referência |
| **Publicação da release** | Quando a versão e suas notas foram formalizadas |
| **Deployment em homologação** | Quando a versão chegou ao ambiente de validação |
| **Deployment em produção** | Quando a versão foi implantada em produção |
| **Disponibilização** | Quando usuários passaram a ter acesso à capacidade |
| **Encerramento/estabilização** | Quando a observação inicial confirmou estabilidade aceitável |

Essas datas podem coincidir, mas não precisam coincidir. O próprio GitHub alerta que a data da tag pode ser diferente da data da release.

Portanto, em vez de perguntar apenas “qual é a data da release?”, a pergunta mais precisa é:

> **Estamos falando da data de corte, da publicação, do deployment em produção ou da disponibilização ao usuário?**

## Exemplo: Release 006

Considere uma organização que usa o nome **Release 006** para consolidar mudanças desde a Release 005.

Uma formulação adequada seria:

> A Release 006 consolida as mudanças selecionadas entre a Release 005 e a data de corte definida, possui uma referência técnica identificável e registra separadamente os deployments realizados por ambiente.

Não seria seguro afirmar:

> Tudo que recebeu commit ou merge no período entrou na Release 006 e chegou à produção.

Podem existir:

- commits em branches que não compõem a versão;
- PRs abertos ou encerrados sem merge;
- mudanças integradas, mas posteriormente revertidas;
- funcionalidades implantadas e desativadas por feature flag;
- componentes implantados em datas diferentes;
- correções emergenciais publicadas fora da janela;
- mudanças técnicas sem impacto visível ao usuário;
- itens concluídos pela gestão, mas ainda não implantados.

## Release não é necessariamente deployment

Uma release pode ser publicada e implantada depois. Uma mesma release pode chegar a homologação e produção em momentos diferentes. Também pode ser implantada progressivamente, por região, cliente ou grupo de usuários.

Da mesma forma, uma organização pode realizar deployments sem criar formalmente uma GitHub Release para cada um deles. A funcionalidade **Releases do GitHub** é uma implementação de plataforma; o conceito organizacional de release pode existir em outros mecanismos.

A transparência depende de registrar pelo menos:

```text
Versão identificada
+ mudanças incluídas
+ ambientes afetados
+ eventos de implantação
+ estado de disponibilização
```

## Release, Sprint e Incremento

Release não é sinônimo de Sprint.

O Scrum Guide estabelece que múltiplos Incrementos podem ser criados dentro de uma Sprint e que um Incremento pode ser entregue antes do fim dela. A Sprint Review não deve ser tratada como uma barreira para liberar valor.

Consequentemente:

- uma Sprint pode produzir mais de um Incremento;
- um Incremento Done pode ser liberado antes da Sprint Review;
- uma release pode reunir trabalho de mais de uma Sprint;
- uma Sprint pode terminar sem que a organização escolha publicar uma release;
- a cadência de aprendizagem não precisa ficar presa à cadência de eventos.

A **Definition of Done** cria transparência sobre a qualidade necessária para que o trabalho faça parte de um Incremento. Ainda assim, a decisão de liberar pode envolver políticas adicionais de produto, risco, operação ou mercado.

## Versionamento não é calendário

Uma versão pode seguir numeração sequencial, como `Release 006`, ou uma convenção como `v1.4.2`.

No Versionamento Semântico, por exemplo:

- **MAJOR** indica mudanças incompatíveis;
- **MINOR** indica funcionalidade compatível;
- **PATCH** indica correções compatíveis.

Esse modelo comunica a natureza da mudança, não o período em que ela foi produzida. Outros contextos podem utilizar versões baseadas em data. O importante é tornar a convenção explícita e aplicá-la consistentemente.

Depois que uma versão é publicada, seu conteúdo não deveria ser alterado silenciosamente. Uma nova mudança deve produzir nova versão, preservando rastreabilidade e capacidade de recuperação.

## A visão técnica e a visão de gestão

| Visão técnica | Visão de gestão |
|---|---|
| Qual código compõe a versão? | Qual objetivo ou resultado está sendo atendido? |
| Qual tag ou commit é a referência? | Qual janela de entrega está sendo comunicada? |
| Quais builds e artefatos foram produzidos? | Quais funcionalidades, correções e mudanças estão incluídas? |
| Em quais ambientes houve deployment? | O que está disponível e para quem? |
| Como fazer rollback ou reproduzir a versão? | Quais riscos, dependências e pendências permanecem? |
| Quais verificações foram executadas? | Qual aprendizado ou impacto foi observado? |

Uma release madura conecta as duas visões. Ela funciona como um **contrato de transparência entre tecnologia, produto e gestão**, e não apenas como um nome numérico ou uma lista de atividades.

## Registro mínimo recomendado

Uma release pode registrar:

1. nome e versão;
2. objetivo ou resultado esperado;
3. período de referência, quando aplicável;
4. data de corte;
5. tag ou commit de referência;
6. Pull Requests e mudanças incluídas;
7. correções, alterações técnicas e migrações;
8. itens explicitamente não incluídos;
9. dependências, riscos e impactos;
10. ambientes e datas de deployment;
11. estado de disponibilização aos usuários;
12. evidências de testes e validação;
13. estratégia de rollback, quando necessária;
14. responsáveis e canais de suporte;
15. métricas e feedback após a liberação.

O nível de detalhe deve ser proporcional ao risco. O objetivo não é burocratizar a entrega, mas permitir que pessoas diferentes respondam com segurança: **o que mudou, qual versão mudou, onde está disponível e que efeito produziu**.

## Relação com métricas de fluxo

Release e deployment oferecem pontos de observação importantes, mas as métricas dependem de fronteiras explícitas.

- **Lead Time**: tempo total entre uma demanda ou compromisso definido e a entrega correspondente.
- **Cycle Time**: tempo entre o início e o término do trabalho, conforme a política do fluxo.
- **Release Frequency**: quantidade de releases em um período.
- **Deployment Frequency**: frequência com que mudanças são implantadas no ambiente definido.
- **Tempo de estabilização**: tempo necessário para atingir estabilidade aceitável depois da implantação.
- **Change Failure Rate**: proporção de mudanças que provocam falha, incidente ou necessidade de correção.

Contar releases sem definir o que a organização chama de release produz uma métrica frágil. Da mesma forma, comparar Lead Time ou Cycle Time entre equipes sem alinhar os pontos de início e fim pode gerar conclusões incorretas.

Ver [Lead Time, Cycle Time, WIP, Aging e Throughput]({{ site.baseurl }}/Métricas-&-Indicadores-(KPI)/Lead-Time,-Cycle-Time,-WIP,-Aging-e-Throughput.html).

## Anti-padrões

- usar commit como prova de entrega;
- tratar merge na branch principal como sinônimo de produção;
- afirmar que toda mudança do período pertence à release sem conferir a referência técnica;
- criar uma release sem tag, commit ou outro identificador reproduzível;
- chamar um relatório retrospectivo de cinco meses de uma única release sem identificar os deployments intermediários;
- alterar silenciosamente o conteúdo de uma versão já publicada;
- transformar Sprint Review em autorização obrigatória para liberar valor;
- medir produtividade pela quantidade de commits;
- comunicar “está em produção” quando a funcionalidade ainda não está disponível aos usuários;
- registrar apenas funcionalidades visíveis e ignorar correções, migrações, riscos e mudanças operacionais.

## Perguntas de diagnóstico

- O que a organização chama de release?
- Existe diferença explícita entre release técnica e janela gerencial?
- Qual referência permite reproduzir a versão?
- Quais datas são registradas?
- É possível provar quais mudanças chegaram a cada ambiente?
- Feature flags e liberações graduais são visíveis para a gestão?
- A Sprint está sendo usada indevidamente como lote obrigatório?
- As notas de release comunicam valor sem perder rastreabilidade técnica?
- Release Frequency e Deployment Frequency estão sendo confundidas?
- O feedback posterior retorna ao upstream e altera prioridades?

## Páginas relacionadas

- [Gestão do Fluxo de Valor]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor.html)
- [Downstream]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Downstream.html)
- [Fluxo End to End]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Fluxo-End-to-End.html)
- [Paralelo com SAFe]({{ site.baseurl }}/Conceitos-Ágeis/Gestão-do-Fluxo-de-Valor/Paralelo-com-SAFe.html)
- [Scrum]({{ site.baseurl }}/Conceitos-Ágeis/Scrum.html)
- [Extreme Programming (XP)]({{ site.baseurl }}/Conceitos-Ágeis/Extreme-Programming-(XP).html)
- [Lead Time, Cycle Time, WIP, Aging e Throughput]({{ site.baseurl }}/Métricas-&-Indicadores-(KPI)/Lead-Time,-Cycle-Time,-WIP,-Aging-e-Throughput.html)

## Referências

- [Git — User Manual](https://git-scm.com/docs/user-manual)
- [Git — git-tag](https://git-scm.com/docs/git-tag)
- [GitHub Docs — About pull requests](https://docs.github.com/en/pull-requests/get-started/about-pull-requests)
- [GitHub Docs — About releases](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases)
- [GitHub Docs — Managing releases](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository)
- [GitHub Docs — Automatically generated release notes](https://docs.github.com/en/repositories/releasing-projects-on-github/automatically-generated-release-notes)
- [Semantic Versioning 2.0.0](https://semver.org/)
- [The Scrum Guide — 2020](https://scrumguides.org/scrum-guide.html)
- [Scrum.org — Evidence-Based Management Guide](https://www.scrum.org/resources/online-evidence-based-management-guide)

## Fontes e proveniência

- Página criada a partir de uma reflexão sobre a diferença entre commits, Pull Requests, merges, releases, deployments e períodos de entrega.
- A situação prática foi generalizada no exemplo “Release 006”, sem expor organização, produto, pessoas ou repositórios profissionais.
- As afirmações técnicas foram confrontadas com documentação oficial do Git, GitHub, Semantic Versioning, Scrum Guide e Scrum.org.
- Onde a terminologia pode variar entre organizações, o conteúdo explicita a diferença entre definição técnica, convenção de governança e inferência.
