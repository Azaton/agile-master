---
title: "Pilha e Fila"
nav_order: 8
parent: "DevTeam"
---

Em desenvolvimento de software, **Fila** e **Pilha** são estruturas de dados que organizam elementos de maneira específica, cada uma com suas próprias regras para adição e remoção de elementos. Essas estruturas são fundamentais para resolver diversos tipos de problemas de programação.

### Pilha (Stack)

Uma **Pilha** é uma estrutura de dados do tipo LIFO (Last In, First Out), o que significa que o último elemento adicionado à pilha será o primeiro a ser removido. Imagine uma pilha de pratos: o último prato colocado no topo é o primeiro a ser retirado. Em termos de operações básicas, uma pilha permite:

- **Push**: Adicionar um elemento no topo da pilha.
- **Pop**: Remover e retornar o elemento do topo da pilha.
- **Peek** ou **Top**: Observar o elemento no topo da pilha sem removê-lo.

Pilhas são usadas em várias situações na computação, como na execução de chamadas de função (onde cada chamada é colocada em uma pilha), na avaliação de expressões (como expressões matemáticas em notação pós-fixa) e em algoritmos de backtracking.

### Fila (Queue)

Uma **Fila** é uma estrutura de dados do tipo FIFO (First In, First Out), significando que o primeiro elemento adicionado será o primeiro a ser removido. Isso é análogo a uma fila de pessoas esperando para serem atendidas em um banco, onde a primeira pessoa que chega é a primeira a ser atendida. As operações básicas em uma fila incluem:

- **Enqueue**: Adicionar um elemento ao final da fila.
- **Dequeue**: Remover e retornar o primeiro elemento da fila.
- **Front**: Observar o primeiro elemento da fila sem removê-lo.

Filas são amplamente utilizadas para gerenciar tarefas em sistemas operacionais, em simulações de eventos (onde eventos são enfileirados e processados na ordem de chegada), e em algoritmos de busca em largura (Breadth-First Search) em grafos.

Ambas as estruturas são fundamentais para a criação de algoritmos eficientes e para a gestão de dados em diversas aplicações de software, desde a implementação de algoritmos complexos até o gerenciamento de recursos em sistemas operacionais.

---

Entendi, você está procurando exemplos mais tangíveis de como os usuários finais interagem indiretamente com o conceito de pilha durante operações comuns em interfaces de usuário (front-end). Vamos a alguns cenários onde a experiência do usuário final reflete o uso subjacente de uma estrutura de pilha:

1. **Navegação de Páginas Web (Botões Voltar e Avançar)**: Quando um usuário navega por páginas na web, clicando em links para avançar e usando o botão "voltar" do navegador para retornar à página anterior, ele está interagindo com uma pilha. O navegador mantém uma pilha das páginas visitadas. Cada nova página visitada é "empilhada" (push) no topo. Quando o usuário clica em "voltar", o navegador "desempilha" (pop) a página atual e retorna à anterior.

2. **Desfazer e Refazer em Aplicativos de Edição**: Em aplicativos de edição de texto, imagem ou vídeo, quando os usuários realizam ações como digitar, apagar, cortar, colar ou aplicar filtros, e depois usam as funções de desfazer (undo) e refazer (redo), eles estão utilizando pilhas. As ações são empilhadas em uma ordem específica, permitindo aos usuários voltar atrás em suas edições passo a passo (desfazendo) ou avançar novamente (refazendo).

3. **Jogos com Funcionalidade de Desfazer**: Em jogos de computador ou aplicativos móveis, especialmente jogos de quebra-cabeça ou de tabuleiro, a opção de desfazer uma jogada permite aos jogadores reverter suas ações. Essa funcionalidade geralmente é implementada com uma pilha, onde cada movimento é registrado. Ao desfazer, o jogo remove a última ação da pilha, retornando ao estado anterior.

4. **Navegação em Aplicativos Móveis**: Muitos aplicativos móveis usam uma estrutura de navegação baseada em pilha para gerenciar telas e páginas. Quando um usuário abre uma nova tela (por exemplo, detalhes de um produto em um app de compras), essa tela é empilhada no topo da navegação. O botão "voltar" desempilha a tela atual, retornando à tela anterior.

5. **Histórico de Comandos em Terminais ou Shells**: Embora seja um pouco mais técnico, muitos usuários finais interagem com terminais ou shells de comando (por exemplo, Bash no Linux/MacOS, Command Prompt no Windows). O histórico de comandos funciona com uma pilha (ou, em algumas implementações, uma lista) onde os comandos digitados são armazenados. Alguns shells permitem que os usuários naveguem pelo histórico de comandos usando teclas de atalho, "desempilhando" os comandos mais recentes.

Esses exemplos mostram como o conceito de pilha, embora seja uma abstração de programação, tem aplicações diretas que afetam a interação do usuário final com software e aplicações no dia a dia, muitas vezes sem que o usuário esteja ciente da complexidade das operações de dados que facilitam sua experiência.

---

A estrutura de dados do tipo Fila (Queue), operando no princípio FIFO (First In, First Out), também tem várias aplicações práticas que afetam diretamente a experiência do usuário final em ambientes de software. Aqui estão alguns exemplos de como os usuários finais podem interagir indiretamente com filas no decorrer de suas atividades:

1. **Atendimento ao Cliente e Sistemas de Chamadas**: Quando você liga para um serviço de atendimento ao cliente e é colocado em espera, você está entrando em uma fila de chamadas. Os clientes são atendidos na ordem em que as chamadas foram recebidas, refletindo o princípio FIFO.

2. **Impressão de Documentos**: Em um ambiente de escritório ou doméstico, quando vários documentos são enviados para uma impressora ao mesmo tempo, eles são colocados em uma fila de impressão. Cada documento é impresso na ordem em que foi recebido, garantindo um processamento justo e sequencial.

3. **Sistemas de Gerenciamento de Filas**: Em locais como bancos, hospitais ou departamentos de atendimento ao cliente, sistemas eletrônicos de gerenciamento de filas permitem que os usuários peguem uma senha e aguardem sua vez. Esses sistemas utilizam filas para organizar o atendimento, assegurando que os usuários sejam atendidos na ordem correta.

4. **Carregamento de Conteúdo em Aplicativos de Streaming**: Quando você assiste a vídeos em plataformas de streaming, o carregamento (ou "buffering") de partes do vídeo pode ser gerenciado por uma fila. Pequenos segmentos do vídeo são carregados sequencialmente para garantir uma reprodução suave, com cada segmento sendo "enfileirado" para processamento na ordem correta.

5. **Processamento de Tarefas em Background de Aplicativos**: Aplicativos móveis e de desktop frequentemente realizam tarefas em background, como sincronização de dados, atualizações ou uploads. Essas tarefas podem ser enfileiradas e processadas uma de cada vez, assegurando que os recursos do sistema sejam utilizados de maneira eficiente e que as tarefas sejam concluídas na ordem em que foram iniciadas.

6. **Pedidos em Sistemas de Comida Online**: Ao fazer um pedido em um aplicativo de entrega de comida, seu pedido é colocado em uma fila de processamento. O restaurante então prepara e entrega os pedidos na ordem em que foram recebidos, aplicando o princípio FIFO para garantir que todos os pedidos sejam atendidos de forma justa e organizada.

7. **Jogos Online Multiplayer**: Em jogos online com sistemas de matchmaking, quando jogadores procuram por partidas, eles podem ser colocados em uma fila até que um número suficiente de jogadores seja encontrado para iniciar o jogo. A fila garante que os jogadores sejam emparelhados para jogos na ordem em que começaram a busca.

Esses exemplos mostram como as filas são usadas em uma ampla variedade de contextos para gerenciar o processamento sequencial de tarefas, atendimento ao cliente, gerenciamento de recursos e muito mais, impactando diretamente a experiência do usuário final em cenários do dia a dia.