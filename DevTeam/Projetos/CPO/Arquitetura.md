---
title: "Arquitetura — CPO"
nav_order: 1
parent: "CPO"
has_children: true
---

# Documentação de Arquitetura do Projeto

---

- **Frontend, Linguagem e Framework**

  - O projeto utiliza **TypeScript** ou **JavaScript** como linguagem de programação.
  - O Frontend é construído usando **React** + **Vite** ou **Next**.
  - Para autenticação, é utilizado o **JWT (JSON Web Tokens)** ou **Login/Auth**.

- **Backend**

  - O servidor web é baseado em **Node.js** com o framework **Fastify**. Avaliar a integração com o **HubSpot**, seja por meio de um pluging ou diretamente através de sua API.
  
- **Banco de Dados**

  - [Prisma](https://www.prisma.io/) (ORM)
  - MySQL (Banco de Dados)

- **Infraestrutura e Hospedagem**

  - Servidor VPS no contabo.com
  - O projeto fará uso de contêineres (**Docker**).
  - Para orquestração desses contêineres, o projeto utilizará **Kubernetes**.

- **Escalabilidade**

  - A aplicação deve ser capaz de suportar **1000 requisições no mês**.
  - Utilizará a capacidade de escalonamento do Kubernetes, provavelmente ajustando o número de pods (instâncias) conforme necessário.

- **Pipeline e Segurança**

  - O projeto seguirá uma abordagem **DevSecOps**, com foco em planejamento e etapas seguras no pipeline do GitLab.