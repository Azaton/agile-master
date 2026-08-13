---
title: "Procedimento de Apontamento de Horas no Azure DevOps"
nav_order: 5
parent: "DevOps"
---

# Introdução

O apontamento de horas é uma prática essencial na gestão de projetos de software e não apenas um exercício administrativo. Ele fornece visibilidade sobre o esforço necessário para concluir tarefas, ajuda na estimativa, previsionar os futuros trabalhos e dá uma visão clara do progresso atual.

É importante dedicarmos de 5 ~ 15 minutos diários para organizarmos as tarefas, e atualizarmos as horas. Ao dedicar este tempo, o resultado reflete  no esforço gasto, as equipes se colocam em uma posição melhor para o sucesso em projetos futuros.

Na organização, cada desenvolvedor é estimado para dedicar 6 horas de trabalho efetivo diariamente. Para uma Sprint de 10 dias, isso resulta em 30 horas por semana ou um total de 60 horas na Sprint por desenvolvedor.

## Passo a Passo para Preenchimento

1. **Acessando a Task**:
    - Navegue até o board do seu projeto no Azure DevOps.
    - Localize a task que deseja atualizar.

2. **Preenchendo o Original Estimate**:
    - Localize o campo "Original Estimate".
    - Digite a quantidade inicial de horas que você estima que serão necessárias para concluir a task. Isso deve ser feito antes de iniciar a task.
    - Esse valor não deve mudar uma vez definido; ele serve como uma referência do que foi originalmente previsto.

3. **Preenchendo o Remaining (Restante)**:
    - Localize o campo "Remaining".
    - Durante a execução da task, atualize esse campo para refletir quantas horas você estima que ainda são necessárias para concluir a task.
    - À medida que você trabalha na task, esse número deve diminuir.

4. **Preenchendo o Completed (Concluído)**:
    - Localize o campo "Completed".
    - À medida que você trabalha na task, atualize esse campo para refletir quantas horas você já trabalhou na task.
    - Esse número deve aumentar proporcionalmente à quantidade de trabalho realizado.

### Importância do Apontamento de Horas:

1. **Visibilidade e Transparência**:
    - O registro de horas ajuda a equipe e os stakeholders a terem uma visão clara do progresso atual.
    - Mostra quanto esforço já foi gasto e quanto esforço ainda é necessário, dando uma ideia do progresso da task.

2. **Estimativa Acurada**:
    - Registrar horas permite que as equipes avaliem a precisão de suas estimativas originais. Com o tempo, isso pode ajudar a melhorar as estimativas futuras.
    - É uma ferramenta vital para retrospectivas. Ao revisar tarefas passadas, as equipes podem entender melhor onde subestimaram ou superestimaram o esforço.

3. **Planejamento Eficiente**:
    - Uma visão clara do esforço necessário para diferentes tarefas permite um planejamento mais informado. Isso é crucial para o planejamento de sprints e definição de prazos.

4. **Responsabilidade**:
    - Registrar horas promove a responsabilidade individual e da equipe. Torna claro o esforço gasto e incentiva a equipe a refletir sobre sua eficiência e produtividade.

5. **Saúde da Equipe**:
    - Se as tarefas consistentemente levam mais tempo do que o estimado, pode ser um sinal de sobrecarga de trabalho, escopo mal definido ou outros problemas que precisam ser abordados.

## Refinamento e Reestimação

**Duração:** Dependendo da complexidade das histórias e das descobertas feitas durante a sprint, pode ser necessário algum tempo (por exemplo, 30 minutos a 1 hora por semana) para refinamentos adicionais ou reestimação.

**Atividade dos Desenvolvedores:** Durante este tempo, os desenvolvedores podem descobrir que uma tarefa é mais complexa do que inicialmente pensado e pode precisar de reestimação. Também pode haver necessidade de dividir uma task ou de adicionar novas tasks.

## Porque das 6 horas?

Estas 6 horas diárias são uma estimativa para preenchermos no Azure, considerando vários aspectos do dia-a-dia do desenvolvedor. Isso inclui, mas não se limita a:

- **Tempo de Almoço**.
- **Cerimônias Scrum**, como Daily Stand-ups, Retrospectivas e Revisões de Sprint.
- **Reuniões de Alinhamentos** com outros membros da equipe ou stakeholders.
- **Refinamentos** de itens do backlog.
- **Organização dos Commits e Branches** nos ambientes.
- **Comunicação e Colaboração** com colegas e outras partes interessadas.
- **Interrupções e Distracções** no ambiente de trabalho.
- **Pausas Regulares** para saúde mental e física.
- **Documentação**, tanto leitura quanto escrita.
- **Aprendizado e Pesquisa** para solucionar problemas ou entender novas tecnologias.
- **Manutenção de Código** e refatoração.
- **Testes Unitários e de Integração**.
- **Gestão de Dependências** e atualizações.
- **Feedback e Iterações** baseadas nas revisões e testes.


1. **Comunicação e Colaboração**:
   - Tempo gasto conversando com colegas de equipe, QA (Quality Assurance), Designers, Product Owners e outros stakeholders.
   - Discussões de código (code reviews) e feedbacks.
   - Assincronias na comunicação, especialmente em equipes remotas ou distribuídas.

2. **Ambiente de Trabalho**:
   - Tempo gasto configurando ou solucionando problemas no ambiente de desenvolvimento.

3. **Pausas e Saúde Mental**:
   - Pequenas pausas durante o dia para descanso mental e físico.
   - Pesquisas têm mostrado que pausas regulares podem aumentar a produtividade e a criatividade.

4. **Documentação**:
   - Tempo gasto lendo ou escrevendo documentação, comentários no código e outros materiais explicativos.

5. **Aprendizado e Pesquisa**:
   - Pesquisando soluções para problemas ou novas tecnologias.
   - Participação em webinars, leitura de blogs, ou acesso a outros recursos educativos.

6. **Manutenção**:
   - Tempo gasto em manutenção de código, refatoração e otimizações.

7. **Testes**:
   - Além da QA, o tempo que os desenvolvedores gastam escrevendo, executando e depurando testes unitários ou de integração.

8. **Gestão de Dependências**:
   - Gerenciando bibliotecas, pacotes e atualizações. Isso pode incluir solução de problemas relacionados a incompatibilidades ou erros.5

9. **Feedback e Iterações**:
   - Ajustes e revisões baseados no feedback do QA, Product Owner ou stakeholders.



