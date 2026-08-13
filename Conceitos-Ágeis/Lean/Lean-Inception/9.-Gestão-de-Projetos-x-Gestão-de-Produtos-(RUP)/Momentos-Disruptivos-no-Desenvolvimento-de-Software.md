---
title: "Momentos Disruptivos no Desenvolvimento de Software"
nav_order: 2
parent: "9. Gestão de Projetos x Gestão de Produtos (RUP)"
---

Houve momentos disruptivos na área de desenvolvimento de software, e o Git, juntamente com ambientes de CI/CD (Integração Contínua/Entrega Contínua), é um exemplo significativo.

### Desenvolvimento de Software Antes do Git

Antes do Git, o desenvolvimento de software utilizava sistemas de controle de versão mais simples e menos colaborativos. Alguns dos sistemas populares incluíam:

1. **RCS (Revision Control System)**: Um dos primeiros sistemas de controle de versão, utilizado principalmente para controle de versão de arquivos individuais.
2. **CVS (Concurrent Versions System)**: Um sistema que permitia a colaboração entre desenvolvedores, mas tinha limitações em termos de fusão de branches e manuseio de arquivos binários.
3. **Subversion (SVN)**: Um avanço significativo sobre o CVS, com melhor suporte para renomear e mover arquivos, mas ainda com uma arquitetura centralizada.

Esses sistemas tinham uma arquitetura centralizada, o que significava que todos os desenvolvedores dependiam de um único servidor para todas as operações de controle de versão. Isso podia causar problemas de desempenho e disponibilidade, além de dificultar a colaboração eficiente em equipes distribuídas.

### A Chegada do Git

O Git, criado por Linus Torvalds em 2005, foi uma revolução no controle de versão devido a várias características:

1. **Descentralização**: Cada desenvolvedor tem uma cópia completa do repositório, incluindo todo o histórico de versões. Isso elimina dependências de um único servidor central.
2. **Branching e Merging Eficientes**: O Git facilita a criação e fusão de branches, permitindo fluxos de trabalho de desenvolvimento mais flexíveis e isolados.
3. **Velocidade**: Operações locais são extremamente rápidas, pois não dependem de comunicação com um servidor central.
4. **Integridade dos Dados**: Cada mudança é armazenada com uma soma de verificação (SHA-1), garantindo a integridade e a rastreabilidade das mudanças.

### Ambientes de CI/CD

Os ambientes de CI/CD trouxeram outra disrupção significativa:

1. **Integração Contínua (CI)**: Envolve a integração frequente do código de todos os desenvolvedores em um repositório compartilhado, seguido de testes automáticos para detectar erros rapidamente.
2. **Entrega Contínua (CD)**: Automatiza o processo de entrega de software, garantindo que o código esteja sempre em um estado que possa ser liberado para produção a qualquer momento.
3. **Desenvolvimento Ágil**: Essas práticas suportam metodologias ágeis, permitindo ciclos de desenvolvimento rápidos e iterativos.

### Impacto na Indústria

A combinação de Git e CI/CD transformou radicalmente a maneira como o software é desenvolvido:

- **Colaboração Melhorada**: Equipes distribuídas podem trabalhar de maneira mais eficiente e paralela.
- **Qualidade de Código**: Testes automatizados e integração contínua ajudam a identificar e corrigir problemas mais cedo.
- **Velocidade de Entrega**: A entrega contínua permite lançamentos frequentes e mais rápidos, respondendo melhor às necessidades dos usuários.

Portanto, sim, a introdução do Git e dos ambientes de CI/CD representou um momento disruptivo significativo na área de desenvolvimento de software, revolucionando práticas de desenvolvimento e permitindo a evolução das metodologias ágeis e DevOps.