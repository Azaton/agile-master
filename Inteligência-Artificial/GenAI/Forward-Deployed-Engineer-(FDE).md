---
title: "Forward Deployed Engineer (FDE)"
nav_order: 2
parent: "GenAI"
---

# Forward Deployed Engineer (FDE)

## O que é

**Forward Deployed Engineer (FDE)** — em português, algo como *engenheiro de soluções alocado junto ao
cliente* — é uma função híbrida entre engenharia de software/IA, consultoria técnica, entendimento de
negócio e implantação no ambiente do cliente.

Um FDE acompanha o problema do cliente do início ao fim: entende o processo real, acessa dados e
sistemas, desenha a arquitetura, programa integrações, implanta, avalia os resultados e transfere a
solução para a operação. A característica que separa um FDE de um consultor ou arquiteto tradicional é a
capacidade técnica de efetivamente **construir e colocar a solução em produção**, não apenas recomendar um
caminho.

Essa descrição coincide com as responsabilidades hoje divulgadas pela [OpenAI](https://openai.com/careers/forward-deployed-engineer-fde-healthcare-sf/)
e pela [Anthropic](https://job-boards.greenhouse.io/anthropic/jobs/5026424008) para o cargo.

## Origem: Palantir e o termo militar

"Forward-deployed" é uma expressão militar registrada desde a década de 1950 (Oxford English Dictionary),
usada para descrever tropas posicionadas de forma permanente perto de uma área de interesse ou conflito —
antes mesmo de o conflito acontecer — para reagir mais rápido e sinalizar presença.

A Palantir emprestou o termo do vocabulário militar por volta dos anos 2000 (fontes públicas divergem
entre 2003 e 2010 para o início exato do modelo). O motivo foi um problema específico: os primeiros
clientes da empresa eram agências de inteligência (CIA, FBI, unidades de inteligência do Exército dos
EUA), que não conseguiam compartilhar dados classificados nem descrever claramente seus requisitos. O
ciclo tradicional de consultoria — levantar requisitos, desenvolver, entregar — não funcionava nesse
contexto. A solução da Palantir foi inserir engenheiros no dia a dia dessas agências, para que
aprendessem observando, testando e construindo em tempo real, com liberação de acesso equivalente à de um
funcionário interno.

O modelo se espalhou depois para provedores de infraestrutura e nuvem, que passaram a alocar
especialistas dentro de grandes clientes corporativos (bancos, varejo, energia) para ajudar na migração de
sistemas legados — um problema semelhante de conhecimento tácito e dados que não se transferem bem por
documentação.

Com a explosão da IA generativa, o mesmo padrão reaparece: empresas de IA (OpenAI, Anthropic, Cohere,
Cognition, entre outras) usam FDEs para ajudar clientes enterprise a aplicar seus modelos a dados
desestruturados e sistemas antigos — o gargalo não é falta de modelo, é falta de quem saiba aplicá-lo ao
problema real do cliente.

## Qual cargo faz isso no Brasil?

Ainda não existe uma tradução ou cargo único consolidado. Esse trabalho aparece hoje principalmente com
estes nomes:

| Cargo usado no Brasil                            | Proximidade com FDE |
| ------------------------------------------------ | -------------------: |
| **AI Solutions Engineer**                        |          Muito alta |
| **Engenheiro de Soluções**                       |                Alta |
| **Consultor Técnico de IA/Dados**                |                Alta |
| **Consultor de Implementação**                   |          Média/alta |
| **Arquiteto de Soluções**                        |          Média/alta |
| **Professional Services Engineer**               |                Alta |
| **Machine Learning Engineer voltado ao cliente** |                Alta |
| **Technical Account Manager**                    |             Parcial |
| **Sales Engineer / Pré-vendas técnico**          |             Parcial |

Já existem vagas brasileiras usando **AI Solution Engineer** — a [Runflow](https://vagas.runflow.ai/), por
exemplo, mantém aberta uma posição com esse título em São Paulo, dentro de uma plataforma que se descreve
como voltada a criar, executar e governar agentes de IA para empresas de médio e grande porte. É uma
correspondência direta com o perfil de FDE.

## A diferença essencial

Um arquiteto ou consultor tradicional pode recomendar:

> "Esta é a arquitetura e este é o caminho."

O FDE precisa ir além:

> "Eu entendi o problema, construí a solução com o cliente, coloquei em produção, medi o resultado e deixei o processo funcionando."

Se a pessoa apenas levanta requisitos, organiza o projeto ou faz apresentações, ela não é FDE. A
característica indispensável é a capacidade técnica de efetivamente construir e implantar a solução.

## FDE e papéis correlatos

FDE não substitui esses papéis; eles cobrem fatias diferentes do mesmo problema de levar uma solução de
IA da ideia à produção:

| Papel                                       | Foco principal                                                        | Constrói e implanta a solução? |
| -------------------------------------------- | ----------------------------------------------------------------------- | :-----------------------------: |
| **Forward Deployed Engineer**               | Descoberta + engenharia + implantação, dentro do ambiente do cliente     | Sim, diretamente                |
| **Delivery Lead**                            | Coordenação de prazo, escopo e time de entrega                          | Não, coordena quem constrói     |
| **AI Delivery Manager**                      | Gestão de portfólio/projetos de IA, priorização, stakeholders            | Não, gerencia quem constrói     |
| **Data & AI Solutions Consultant**           | Diagnóstico de negócio e desenho de solução de dados/IA                 | Parcial — desenha, nem sempre implementa |
| **AI Solutions Consultant / AI Deployment Strategist** | Combina entendimento de negócio com prototipação prática e acompanhamento da implantação | Parcial a alto, dependendo do quanto assume hands-on |

Na prática, muitos profissionais que hoje atuam como Delivery Lead, AI Delivery Manager ou Solutions
Consultant já cobrem parte do escopo de um FDE (proximidade com o cliente, tradução entre negócio e
time técnico, acompanhamento da implantação). A diferença que efetivamente separa esses papéis do FDE é a
frequência com que a pessoa prototipa, programa integrações, configura infraestrutura e coloca a solução
em produção com as próprias mãos, em vez de coordenar quem faz isso.

## O que continua relevante para quem quer atuar como FDE

Independentemente do nome do cargo, a combinação de base é: fundamentos de computação e de machine
learning, engenharia de software (padrões de código, arquitetura, escala, segurança) e habilidades de
relacionamento com cliente (comunicação, vendas, customer success). Entender superficialmente como
funciona um token, uma rede neural ou um LLM deixa de ser opcional — sem isso, o profissional trata o
modelo como caixa-preta e não consegue extrair seu potencial nem configurá-lo com segurança dentro de uma
empresa.

## Leitura crítica

O modelo FDE identifica uma tendência real, mas não é uma função inteiramente nova: já existia no Brasil
em consultorias, provedores de nuvem e empresas de dados, sob outros nomes. O que está mudando agora é a
consolidação de um nome único e sua especialização em IA generativa — e a velocidade com que o modelo está
sendo adotado por startups de IA, inclusive brasileiras, que atendem clientes enterprise.

## Páginas relacionadas

- [Profissões e Papéis](./Profissões-e-Papéis.md)
- [Engenharia de Software com GenAI e IA Agêntica](./Engenharia-de-Software-com-GenAI-e-IA-Agentica.md)

## Fontes

- OpenAI. **"Forward Deployed Engineer (FDE), Healthcare"** (vaga): https://openai.com/careers/forward-deployed-engineer-fde-healthcare-sf/
- Anthropic. **"Forward Deployed Engineer"** (vaga): https://job-boards.greenhouse.io/anthropic/jobs/5026424008
- Runflow. **"AI Solution Engineer"** (vaga, São Paulo): https://vagas.runflow.ai/
- Oxford English Dictionary. **"forward-deployed, adj."** (etimologia): https://www.oed.com/dictionary/forward-deployed_adj
- The Pragmatic Engineer. **"What are Forward Deployed Engineers, and why are they so in demand?"**: https://newsletter.pragmaticengineer.com/p/forward-deployed-engineers
- Perspective AI. **"Palantir's Forward-Deployed Engineering Playbook: The Original Model Anthropic and OpenAI Are Copying"**: https://getperspective.ai/blog/palantir-forward-deployed-engineering-playbook-anthropic-openai-copying
- Transcrição de vídeo/podcast enviada como fonte inicial para esta página (canal e autor não identificados
  no material recebido) — usada para a linha do tempo Palantir → provedores de nuvem → empresas de IA e
  para a observação sobre a chegada do modelo ao Brasil.

## Proveniência e confiança

A definição de FDE e a tabela de cargos brasileiros partiram de uma transcrição de vídeo/podcast enviada
como fonte, sem identificação de canal ou autor — por isso as afirmações do vídeo (datas, presença do
termo no Brasil, previsão de crescimento da demanda) foram tratadas como hipótese e confrontadas com fontes
públicas antes de entrar na página.

**Confiança alta:** origem do termo "forward-deployed" no vocabulário militar; adoção pioneira pela
Palantir para lidar com clientes de inteligência que não podiam compartilhar dados nem definir requisitos;
adoção do mesmo modelo por OpenAI e Anthropic hoje.

**Confiança moderada:** ano exato em que a Palantir criou o modelo (fontes públicas divergem entre 2003 e
2010); extensão atual da adoção do termo "FDE" especificamente no Brasil — a evidência direta encontrada
foi uma vaga (Runflow); a tendência mais ampla é uma observação do vídeo-fonte, ainda sem múltiplas fontes
independentes que a confirmem.

Data da última revisão: 2026-09-11
