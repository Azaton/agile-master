---
title: "Modelo Relacionamento de Entidade Aprimorado"
nav_order: 5
parent: "Modelagem e Banco de Dados"
---

**Modelo EER**

O Modelo EER (Modelo de Entidade-Relacionamento Aprimorado) é um design de modelo de dados que captura mais tipos de semântica em um banco de dados do que o modelo tradicional de Entidade-Relacionamento. Ele introduz conceitos como tipos de entidade, conjuntos de entidades e classes, onde uma classe pode conter duas subclasses e subtipos. A Classe Mãe se refere à classe principal ou entidade de onde as outras classes (Classe Filha, Classe Filho) derivam e herdam características.

**Herança**

No contexto dos bancos de dados EER, a herança é um princípio que permite que as entidades compartilhem atributos comuns, significando que as subclasses (ou entidades filho) podem herdar características da superclasse (ou entidade mãe). Isso é particularmente útil no mapeamento objeto-relacional, também conhecido como PPO (Persistência Poliglota Orientada), onde os objetos de uma aplicação são mapeados e armazenados em um banco de dados. Essa herança ajuda a evitar a redundância e promove a consistência dos dados.

**Especialização e Generalização**

A especialização é um processo de definição de um conjunto de subclasses a partir de uma superclasse, identificando suas características ou atributos especiais. A generalização é o processo inverso, agrupando propriedades comuns de várias subclasses para formar uma superclasse. Ambos são processos de abstração que ajudam a lidar com a complexidade em modelos de banco de dados. Eles permitem mapear instâncias das superclasses e subclasses em relação ao mundo real, enfatizando o papel especializado de cada entidade e seus relacionamentos específicos.

**Constraints de Generalização e Especialização - parte 1**

As restrições de generalização e especialização definem regras que estabelecem condições para o relacionamento entre superclasses e subclasses em um modelo EER. Algumas das principais restrições incluem:

- **Attribute-defined specialization**: Ocorre quando a especialização é definida com base em algum atributo da superclasse. Por exemplo, um funcionário pode ser especializado em Gerente ou Operador com base no atributo "cargo".
  
- **User-defined specialization**: Esta é uma especialização onde a divisão em subclasses é determinada pelo usuário ou pelo aplicativo, não baseada em atributos.
  
- **Predicate-defined specialization**: Ocorre quando a especialização é definida com base em uma condição (ou predicado). Por exemplo, um cliente pode ser dividido em Clientes Premium e Clientes Regulares com base no saldo de crédito.

- **Disjointness constraint (Restrição de disjunção)**: Define se uma instância da superclasse pode pertencer a uma ou mais subclasses. No caso de "disjoint" (disjunção), uma instância só pode pertencer a uma subclasse. No caso de "overlapping", uma instância pode pertencer a várias subclasses.

- **Completeness constraint (Restrição de completude)**: Define se uma instância da superclasse deve pertencer a pelo menos uma subclasse ("total") ou pode não pertencer a nenhuma subclasse ("partial").

As restrições de integridade também são aplicadas durante as operações de inserção e exclusão para garantir a consistência dos dados.

**Hierárquia & Rede de Especialização**

No livro de Navathe, a Hierarquia e Rede de Especialização referem-se à estrutura organizacional de entidades em um modelo EER. Uma hierarquia de especialização é uma árvore estruturada de superclasses e subclasses, enquanto uma rede de especialização permite que uma classe seja subdividida em várias formas, e uma subclasse pode ser parte de várias superclasses.

**Modelagem de Union Types usando Categorias**

"Union Types" ou "Tipos de União" referem-se a uma situação em que uma entidade pode ser de um tipo ou de outro. No livro de Navathe, é abordada a ideia de modelagem de tipos de união usando categorias. Uma categoria permite agrupar entidades de diferentes conjuntos de entidades que possuem atributos comuns. Por exemplo, uma entidade "Pessoa" pode ser um "Funcionário" ou um "Cliente", e os atributos comuns podem ser agrupados na categoria "Pessoa".

**Esquema EER & Definições formais**

Um esquema EER (Modelo de Entidade-Relacionamento Aprimorado) é uma representação abstrata e conceitual do banco de dados, que inclui entidades, relacionamentos, atributos e restrições. Ele estabelece as definições formais para a organização e estrutura dos dados em um banco de dados. O esquema EER é mais expressivo que o modelo ER tradicional, pois incorpora conceitos como herança, especialização, generalização e categorias, permitindo uma descrição mais precisa e completa do domínio do problema.

**Decisão sobre Design de BD & UML**

As decisões sobre o design do banco de dados são influenciadas por vários fatores, incluindo as necessidades de informação dos usuários, o volume de dados, o desempenho, a segurança, entre outros. O UML (Unified Modeling Language), que é uma linguagem de modelagem visual padrão, é frequentemente utilizada no processo de design do banco de dados. Os diagramas UML, como o diagrama de classes, podem ser usados para visualizar a estrutura do banco de dados, facilitando a compreensão e a comunicação das decisões de design.