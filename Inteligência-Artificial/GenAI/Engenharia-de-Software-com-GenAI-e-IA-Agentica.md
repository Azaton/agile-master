---
title: "Engenharia de Software com GenAI e IA Agêntica"
nav_order: 1
parent: "GenAI"
---

# Engenharia de Software com GenAI e IA Agêntica

> Da geração assistida à execução governada ao longo do ciclo de desenvolvimento.

A Inteligência Artificial está provocando uma mudança estrutural na Engenharia de Software. O movimento começou com ferramentas capazes de sugerir código, explicar funções e produzir documentação. Agora, avança para sistemas que recebem objetivos, consultam fontes, utilizam ferramentas e executam sequências de ações.

Essa transformação não representa apenas uma maneira mais rápida de programar. Ela modifica a relação entre intenção, especificação, execução, validação e governança.

O modelo de linguagem deixa de ser somente uma interface de perguntas e respostas e passa a integrar uma arquitetura composta por contexto, memória, ferramentas, agentes, controles e observabilidade. O desafio central não é gerar mais código, mas construir sistemas capazes de contribuir para a entrega de valor com segurança, qualidade e responsabilidade.

## Da assistência para a atuação agêntica

GenAI e IA agêntica são conceitos relacionados, mas não equivalentes.

A **Inteligência Artificial Generativa** produz novos conteúdos a partir de uma instrução e do contexto recebido. Ela pode criar textos, códigos, testes, diagramas, análises e documentação.

A **IA agêntica** acrescenta capacidade de atuação: o sistema interpreta um objetivo, organiza etapas, escolhe ferramentas, executa ações, observa resultados e ajusta o próximo passo. Dependendo dos limites definidos, pode solicitar aprovação humana antes de realizar operações sensíveis.

| Estágio | Atuação da IA | Responsabilidade humana |
|---|---|---|
| Desenvolvimento tradicional | Participação indireta ou inexistente | Especificar, implementar e validar |
| Desenvolvimento assistido por GenAI | Sugerir, explicar e gerar artefatos | Orientar, revisar e decidir |
| Desenvolvimento agêntico | Planejar e executar sequências de ações | Definir objetivos, limites e critérios de aceitação |

Um sistema também pode reunir vários agentes especializados. Nesse caso, diferentes papéis — como análise, implementação, testes, segurança ou documentação — cooperam sob uma forma de coordenação.

A multiplicação de agentes, porém, não garante qualidade. Sem responsabilidades claras, o sistema apenas distribui ambiguidades, aumenta o custo de coordenação e amplia sua superfície de risco.

## Uma mudança em todo o ciclo de desenvolvimento

A aplicação de IA não precisa ficar restrita à codificação. Ela pode apoiar todas as etapas do ciclo de desenvolvimento.

### 1. Descoberta e requisitos

A IA pode organizar entrevistas, documentos e regras de negócio; identificar conflitos; levantar perguntas e transformar necessidades em hipóteses ou requisitos verificáveis.

Ela não determina sozinha qual problema merece ser resolvido. Priorização, valor, impacto e responsabilidade continuam dependendo das pessoas envolvidas e do contexto organizacional.

### 2. Especificação técnica

Uma necessidade pode ser convertida em critérios de aceitação, contratos, modelos de dados, restrições arquiteturais e estratégias de teste. Essa etapa ganha importância porque agentes executam melhor quando recebem objetivos e fronteiras verificáveis.

Quanto maior a autonomia concedida à IA, maior deve ser a clareza da especificação.

### 3. Implementação

Sistemas generativos podem criar e alterar código, explicar componentes, aplicar padrões e auxiliar em refatorações. Sistemas agênticos podem navegar pelo repositório, identificar dependências, modificar diferentes arquivos e executar ferramentas de desenvolvimento.

O aumento da capacidade de execução exige controle de escopo: quais arquivos podem ser alterados, quais comandos são permitidos e quais decisões precisam de aprovação?

### 4. Testes e revisão

A IA pode sugerir testes, analisar cenários de borda, executar verificações e revisar alterações. Ainda assim, um teste gerado pelo mesmo raciocínio que produziu a solução pode repetir suas premissas equivocadas. Revisão independente, evidências objetivas e critérios de aceitação permanecem necessários.

### 5. Deploy e operação

Agentes podem apoiar pipelines, interpretar logs, investigar incidentes e organizar procedimentos operacionais. Em ambientes reais, essas ações devem respeitar segregação de funções, permissões mínimas, rastreabilidade e mecanismos de interrupção.

### 6. Aprendizado e evolução

Os resultados da operação podem alimentar a melhoria do produto, das instruções, das bases de conhecimento e dos controles. Esse aprendizado não deve acontecer de maneira indiscriminada: dados, decisões e feedbacks precisam de origem conhecida, qualidade e autorização de uso.

## Arquitetura de um sistema GenAI e agêntico

Um modelo de linguagem é apenas um componente. Uma solução confiável depende da combinação de diferentes camadas.

| Camada | Responsabilidade |
|---|---|
| Experiência | Interfaces pelas quais pessoas ou sistemas apresentam objetivos e acompanham resultados |
| Orquestração | Controle do fluxo, do estado, das etapas e das aprovações |
| Agentes | Papéis especializados, objetivos delimitados e políticas de atuação |
| Modelos | Geração, interpretação, classificação, planejamento e análise |
| Contexto e conhecimento | Documentos, regras, memória, dados e recuperação de informações |
| Ferramentas e integrações | APIs, repositórios, bancos, pipelines e sistemas corporativos |
| Governança e segurança | Identidade, permissões, guardrails, políticas e intervenção humana |
| Observabilidade | Logs, rastreabilidade, avaliações, qualidade, desempenho e custos |

Essa separação evita um erro recorrente: atribuir ao modelo responsabilidades que pertencem à arquitetura. O modelo pode interpretar uma solicitação, mas o sistema deve controlar acesso, validar entradas e saídas, registrar ações e impedir operações fora da autoridade concedida.

A organização detalhada de contexto, habilidades, integrações e automações é aprofundada em [IA Operacional — Framework CHIA](./IA-Operacional-Framework-CHIA.md). Já os padrões de orquestração, estado, transições e coordenação são tratados em [Engenharia de Grafos](./Engenharia-de-Grafos.md).

## Contexto, ferramentas e conhecimento

Nenhum agente conhece automaticamente a realidade de uma organização. Para atuar de forma útil, ele precisa receber contexto adequado: objetivo, regras de negócio, padrões técnicos, documentação, decisões anteriores, estado atual, critérios de aceitação e restrições.

Técnicas de recuperação de informação, frequentemente reunidas sob o conceito de **RAG**, permitem localizar conteúdos relevantes antes de produzir uma resposta ou tomar uma decisão. A memória pode preservar determinados estados e aprendizados ao longo do fluxo.

Mais contexto, entretanto, não significa necessariamente melhor resultado. Informações antigas, conflitantes ou sem procedência podem induzir decisões erradas. A arquitetura precisa selecionar, versionar e rastrear as fontes utilizadas.

Para produzir efeitos fora da conversa, agentes também precisam utilizar ferramentas. Elas podem permitir consulta a documentos, leitura de repositórios, execução de testes, atualização de tarefas ou interação com sistemas corporativos.

O **Model Context Protocol (MCP)** oferece uma forma padronizada de apresentar ferramentas e recursos a aplicações baseadas em modelos. Ele não substitui APIs, bancos de dados ou regras de autorização. Seu papel é criar uma interface comum entre a aplicação de IA e as capacidades que ela poderá utilizar.

Toda integração precisa esclarecer:

- quem solicita a ação;
- qual agente está atuando;
- qual ferramenta pode ser usada;
- quais dados podem ser acessados;
- quais ações exigem confirmação;
- como o resultado será validado e auditado.

## Desenvolvimento orientado por especificações

Durante décadas, parte relevante da especificação permaneceu implícita na experiência das pessoas e nas conversas do time. Quando agentes passam a executar tarefas, esse conhecimento precisa tornar-se mais claro, estruturado e verificável.

Uma boa especificação para trabalho assistido ou executado por IA deve informar:

- o problema e o resultado esperado;
- o contexto necessário;
- o que está dentro e fora do escopo;
- as restrições técnicas e organizacionais;
- os padrões que devem ser seguidos;
- os critérios de aceitação;
- os testes e evidências esperados;
- as ações permitidas;
- as condições que exigem aprovação humana.

Isso não significa retornar a documentos extensos e imutáveis. A especificação pode evoluir iterativamente. O ponto central é que objetivos e limites precisam ser compreensíveis tanto para pessoas quanto para sistemas.

## O papel humano não desaparece: ele se desloca

A automação reduz parte do esforço operacional, mas amplia a importância do julgamento. O profissional deixa de concentrar seu valor apenas na produção direta de artefatos e passa a atuar também como:

- formulador do problema;
- curador de contexto;
- projetista de especificações;
- supervisor de agentes;
- avaliador crítico de resultados;
- responsável por riscos e decisões.

Na gestão de produtos e projetos, a IA pode apoiar planejamento, documentação e acompanhamento. Porém, não possui legitimidade organizacional para decidir sozinha prioridades, assumir compromissos ou arbitrar interesses humanos.

Na agilidade, isso reforça uma ideia importante: automação não substitui empirismo. Transparência, inspeção e adaptação continuam necessárias, agora aplicadas também ao comportamento dos sistemas inteligentes.

Essa transformação também favorece profissionais capazes de conectar negócio e tecnologia, tema desenvolvido em [Purple People](./Purple-People.md) e [Profissões e Papéis](./Profissões-e-Papéis.md).

## Governança antes da escala

Sistemas agênticos ampliam a capacidade de ação e, consequentemente, o impacto de uma falha. Entre os riscos estão uso indevido de ferramentas, instruções maliciosas, exposição de dados, decisões sem rastreabilidade e ações que ultrapassam a intenção original.

O NIST organiza a gestão de riscos de IA em quatro funções: **Governar, Mapear, Medir e Gerenciar**. Essa lógica integra responsabilidade e avaliação ao ciclo de vida, em vez de tratar governança como uma aprovação final.

Alguns controles tornam-se especialmente importantes:

- identidade e autorização por ação;
- privilégio mínimo;
- separação entre ambientes;
- validação de entradas e saídas;
- limites de escopo, custo e tempo;
- aprovação humana para ações sensíveis;
- registro das decisões e ferramentas utilizadas;
- testes contra comportamentos inesperados;
- mecanismos de pausa, reversão e encerramento.

Governança não deve significar paralisia. Seu objetivo é permitir evolução com limites conscientes e evidências suficientes para aprender com segurança.

## Produtividade precisa ser medida como sistema

Gerar código mais rapidamente não significa entregar mais valor. O ganho local pode ser anulado por revisão excessiva, defeitos, retrabalho, complexidade ou aumento do custo operacional.

Uma avaliação equilibrada deve combinar indicadores como:

- tempo de fluxo e tempo de ciclo;
- frequência e confiabilidade das entregas;
- defeitos e retrabalho;
- qualidade e manutenibilidade;
- tempo de revisão;
- incidentes e riscos;
- custo de modelos e infraestrutura;
- adoção e satisfação das pessoas;
- valor percebido pelo cliente ou usuário.

Antes de atribuir um ganho à IA, é necessário estabelecer uma linha de base, observar o fluxo completo e separar percepção de evidência. Percentuais publicados por fornecedores ou pesquisas devem ser interpretados conforme amostra, tarefa, experiência dos participantes e método de medição.

## Uma jornada incremental de adoção

### 1. Diagnóstico

Mapear o fluxo atual, suas dores, métricas, riscos e restrições. O objetivo não é procurar onde inserir IA, mas descobrir onde existe um problema relevante que ela possa ajudar a resolver.

### 2. Experimento controlado

Selecionar um caso de uso delimitado, definir uma linha de base e estabelecer critérios de sucesso. Manter revisão humana e registrar falhas, ganhos e efeitos colaterais.

### 3. Integração ao fluxo

Conectar a solução aos repositórios, documentos, testes e sistemas necessários. Formalizar identidade, permissões, aprovações e observabilidade.

### 4. Escala governada

Expandir somente após validar utilidade, segurança e sustentabilidade. Criar práticas de treinamento, avaliação contínua, gestão de custos e resposta a incidentes.

## Uma mudança maior do que uma nova ferramenta

A Engenharia de Software com GenAI e IA agêntica não deve ser compreendida como a simples substituição de ferramentas tradicionais. Trata-se de uma nova distribuição do trabalho entre pessoas e sistemas.

As organizações mais preparadas não serão necessariamente aquelas que gerarem mais código, mas as que conseguirem transformar conhecimento em boas especificações, conceder autonomia de maneira proporcional ao risco e preservar responsabilidade sobre as decisões.

O futuro da Engenharia de Software tende a ser menos definido pela oposição entre humanos e máquinas e mais pela qualidade da cooperação entre ambos. A tecnologia amplia possibilidades; propósito, discernimento e responsabilidade continuam determinando quais possibilidades devem tornar-se realidade.

## Páginas relacionadas

- [Engenharia de Grafos](./Engenharia-de-Grafos.md)
- [IA Operacional — Framework CHIA](./IA-Operacional-Framework-CHIA.md)
- [Profissões e Papéis](./Profissões-e-Papéis.md)
- [Purple People](./Purple-People.md)
- Engenharia de Contexto — expansão futura
- Sistemas Multiagentes — expansão futura
- Observabilidade e Avaliação de Agentes — expansão futura

## Fontes

- NIST. **Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile**: https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-generative-artificial-intelligence
- NIST. **AI Risk Management Framework**: https://www.nist.gov/itl/ai-risk-management-framework
- Model Context Protocol. **Documentação oficial**: https://modelcontextprotocol.io/docs/
- OWASP. **AI Agent Security Cheat Sheet**: https://cheatsheetseries.owasp.org/cheatsheets/AI_Agent_Security_Cheat_Sheet.html
- OWASP. **Agentic AI — Threats and Mitigations**: https://genai.owasp.org/resource/agentic-ai-threats-and-mitigations/

## Proveniência e confiança

Este conteúdo foi elaborado a partir de uma apresentação sobre a evolução da Engenharia de Software apoiada por IA. Marcas, produtos e propostas comerciais foram removidos para preservar uma leitura pública, conceitual e independente de fornecedor. As definições arquiteturais e os controles foram confrontados com referências do NIST, do Model Context Protocol e da OWASP.

**Confiança alta:** distinção entre geração e atuação, arquitetura em camadas, necessidade de contexto, ferramentas, permissões, observabilidade e supervisão humana.

**Confiança moderada:** consolidação de “Engenharia de Software Agêntica” como denominação estável de uma disciplina. Em 2026, o termo ainda representa um campo em rápida formação.
