---
title: "Antes do Git e da adoção de CICD"
nav_order: 1
parent: "9. Gestão de Projetos x Gestão de Produtos (RUP)"
---

Antes do Git e da adoção ampla de práticas de CI/CD, os projetos de desenvolvimento de software geralmente seguiam metodologias diferentes das ágeis, como o modelo em cascata (waterfall). Para fazer um paralelo entre o cenário anterior e o atual, vamos analisar algumas diferenças principais em termos de tipos de projetos e metodologias.

### Projetos Antes do Git e CI/CD

**Metodologias Tradicionais:**
1. **Modelo em Cascata (Waterfall):**
   - **Planejamento Extenso**: Cada fase do desenvolvimento (requisitos, design, implementação, testes, manutenção) era completada antes de passar para a próxima.
   - **Pouca Flexibilidade**: Mudanças nos requisitos eram difíceis de incorporar após o início do projeto.
   - **Lançamentos Infrequentes**: O software era geralmente liberado apenas no final de um ciclo de desenvolvimento completo, levando meses ou até anos.

**Ferramentas e Práticas:**
1. **Controle de Versão Centralizado (ex: SVN, CVS):**
   - **Dependência de Servidor Central**: Repositórios centralizados limitavam a colaboração eficiente, especialmente em equipes distribuídas.
   - **Branching e Merging Complicados**: Fusões de branches eram complexas e propensas a erros, desestimulando a criação de branches para novas funcionalidades.

2. **Processos Manuais:**
   - **Deploy Manual**: A implantação de software era frequentemente feita manualmente, aumentando o risco de erros.
   - **Testes Manuais**: Muitos testes eram realizados manualmente, o que era demorado e sujeito a falhas humanas.

### Projetos Após o Git e CI/CD

**Metodologias Ágeis:**
1. **Scrum, Kanban e XP (Extreme Programming):**
   - **Iterações Curtas (Sprints)**: Desenvolvimento ocorre em ciclos curtos, permitindo a entrega frequente de incrementos de software.
   - **Feedback Contínuo**: Incorporar feedback dos usuários e stakeholders continuamente.
   - **Flexibilidade**: Requisitos podem ser ajustados com base em feedback e mudanças de mercado.

**Ferramentas e Práticas:**
1. **Controle de Versão Distribuído (Git):**
   - **Branching e Merging Simples**: Facilita a criação de branches para novas funcionalidades e fusões frequentes, suportando desenvolvimento paralelo.
   - **Histórico Completo Local**: Cada desenvolvedor tem acesso ao histórico completo do repositório, facilitando o trabalho offline e revisões de código.

2. **CI/CD:**
   - **Integração Contínua (CI)**: Código é integrado e testado automaticamente, reduzindo o tempo de detecção de erros.
   - **Entrega Contínua (CD)**: Automatiza o deploy de software, permitindo lançamentos frequentes e confiáveis.
   - **Automação de Testes**: Testes automatizados garantem que novas mudanças não quebrem funcionalidades existentes.

### Paralelo dos Tipos de Projetos

**Antes do Git e CI/CD:**
- **Projetos Longos e Rígidos**: Seguiam um planejamento detalhado no início e tinham dificuldade em se adaptar a mudanças.
- **Menos Colaboração**: Desenvolvimento mais isolado e centralizado.
- **Deploy Infrequente**: Novas versões do software eram lançadas menos frequentemente, resultando em ciclos de feedback mais longos.

**Depois do Git e CI/CD:**
- **Projetos Ágeis e Iterativos**: Adotam ciclos curtos de desenvolvimento com entregas incrementais.
- **Alta Colaboração**: Facilita o trabalho colaborativo em equipes distribuídas e a integração frequente de código.
- **Deploy Frequente**: Lançamentos contínuos e automação permitem responder rapidamente às necessidades dos usuários.

### Conclusão

O Git e os ambientes de CI/CD não só facilitaram a adoção de metodologias ágeis, mas também transformaram a maneira como os projetos de software são gerenciados, promovendo colaboração, flexibilidade e entregas rápidas e contínuas. Essas mudanças tornaram o desenvolvimento de software mais dinâmico e eficiente, adaptando-se melhor às necessidades de um mercado em constante evolução.