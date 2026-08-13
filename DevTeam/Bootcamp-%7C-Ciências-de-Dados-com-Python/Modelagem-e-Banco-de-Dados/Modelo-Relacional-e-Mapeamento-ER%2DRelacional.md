---
title: "Modelo Relacional e Mapeamento ER Relacional"
nav_order: 4
parent: "Modelagem e Banco de Dados"
---

**Conceitos de Modelo Relacional: Tupla, Atributo e Relação - Parte 1**

O esquema relacional define a estrutura de uma base de dados relacional, incluindo os nomes das tabelas, os campos (ou atributos) que cada tabela contém, e as relações entre os campos de diferentes tabelas. O atributo (AI) representa uma característica ou propriedade de uma entidade, enquanto o domínio (D) representa o conjunto de valores permitidos para um atributo.

Por exemplo, se tivermos uma tabela "Cliente" no esquema relacional, esta pode ter atributos como "Nome", "Endereço", "Número de Telefone", cada um com seu próprio domínio: "Nome" pode ser uma string de até 50 caracteres, "Endereço" pode ser uma string de até 200 caracteres, e "Número de Telefone" pode ser um número inteiro de até 11 dígitos.

**Conceitos de Modelo Relacional: Tupla, Atributo e Relação - Parte 2**

Uma relação em um modelo relacional é uma tabela composta de tuplas (ou linhas) e atributos (ou colunas). Essa organização permite o armazenamento de dados de maneira estruturada e ordenada.

As tuplas dentro de uma relação representam um conjunto de dados relacionados. Por exemplo, em uma tabela "Cliente", cada tupla poderia representar um cliente específico, com os atributos fornecendo informações detalhadas sobre aquele cliente.

Os arquivos, nesse contexto, representam o local físico onde os dados das tabelas são armazenados, enquanto as tabelas são as estruturas lógicas que organizam esses dados. A ordenação de tuplas na relação pode ser crucial para eficiência de buscas e recuperação de dados. Isso pode envolver a ordenação das tuplas com base em um ou mais atributos, facilitando a localização rápida de dados específicos dentro da relação.

**Conceitos de Modelo Relacional: Cardinalidade, Domínio e Relação**

A cardinalidade refere-se ao número de ocorrências em uma relação de um modelo relacional. Por exemplo, em uma relação entre duas tabelas "Cliente" e "Pedido", a cardinalidade poderia ser 'um-para-muitos', indicando que um cliente pode ter muitos pedidos.

O domínio é o conjunto de valores possíveis que um atributo pode ter. Por exemplo, o domínio do atributo "idade" em uma tabela "Cliente" pode ser qualquer número inteiro positivo.

A relação em um modelo relacional é uma tabela que contém tuplas e atributos. As tuplas (linhas) representam registros individuais, enquanto os atributos (colunas) representam os diferentes tipos de informações que são armazenadas sobre cada registro.

**Conceitos de Modelo Relacional: Conjunto de Tuplas**

Um conjunto de tuplas representa todos os registros dentro de uma determinada relação. Cada tupla é um conjunto ordenado de valores, cada um pertencente a um domínio específico, representando um objeto singular na relação.

A ordenação de valores dentro de uma tupla pode ser crítica para a eficiência de buscas e recuperações de dados. Isso poderia envolver a ordenação dos valores de um atributo específico. Por exemplo, se a tupla representa um cliente, os valores do atributo 'sobrenome' podem ser ordenados alfabeticamente para facilitar a busca por um cliente específico.
