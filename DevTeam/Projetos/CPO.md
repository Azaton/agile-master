---
title: "CPO"
nav_order: 2
parent: "Projetos"
has_children: true
---

# Objetivo

Desenvolver um sistema para que os usuários façam agendamentos de forma autônoma. A ideia é desenvolver um site, onde o usuário acessar, selecionada a data e faz a reserva.

# AS IS (cenário atual)

Atualmente o agendamento é feito de forma manual pelo Telegram.

1. Uma mensagem é enviada pelo administrador do grupo Telegram, informando os dias e horários para os usuários fazerem a sua reserva.

2. Os usuários visualizam a mensagem no grupo Telegram.

3. Os usuários são orientados a falar com uma pessoa responsável pelo agendamento.

4. Os usuários visualizam os dias e horários disponíveis, para decidirem qual dia irão participar.

5. Os usuários enviam os dados: Nome Completo, Telefone e E-mail, para o administrador responsável.

6. O administrador do grupo recebe as informações de forma individual e organiza a lista de presença.

7. O administrador imprimi a lista de presença pelo menos um dia antes das visitas.

# TO BE (cenário futuro)

Entregar um website para que os usuários façam o agendamento das visitas de forma autônoma. Eles acessam a plataforma e, através de uma calendário, selecionam o dia, local e horário da visita.

## Usuário da Plataforma

Usuário da Plataforma são aqueles que fazem a reserva. Após autenticado na plataforma, um calendário estará disponível para agendamento.

1. O usuário acessa o site e utiliza o e-mail para logar no ambiente. Este acesso pode ser direto pela tela de Login ou pela Landing Page.

2. Se o usuário ainda não estiver cadastro, o sistema exibe uma mensagem para o usuário solicitando o cadastramento.

> Usuário informa Nome Completo, E-mail e Telefone/Celular para o cadastramento.
> Usuário informa a senha e confirmação da senha.
> Usuário é direcionado para a tela principal

3. Usuário informa e-mail completo e senha cadastrada.

4. Usuário autenticado, visualiza o calendário.

5. Usuário selecionada a data e horário de agendamento.
> Usuário pode selecionar apenas UMA DATA e HORÁRIO, no dia escolhido.
> Usuário cadastro tem 3 corações no mês. Se ele faltar na data, perde um coração e pode ser penalizado e não conseguir fazer agendamentos dentro de um período de tempo.

6. Dado a reserva, o usuário conseguirá visualizar a data da reserva que foi feita. Um e-mail pode ser disparado para ele ter a confirmação da reserva. Esta comunicação por e-mail pode ser feita em qualquer momento, quando confirmado, alterado ou cancelada uma reserva. A reserva pode ser cancelada um dia antes da visita.

7. Os usuários poderão ser bloqueados pelos administradores.
> Um usuário bloqueado consegue logar na plataforma, mas não consegue fazer um agendamento
> O usuário que desejar ser desbloqueado, poderá fazer a requisição juto ao suporte da CPO.

## Usuários Administrador

O usuário administrador é aquele que terá acesso a lista de reservas. A principal função é conseguir imprimir a lista para fazer a conferência das pessoas, quando elas chegam para assistir uma palestra.

1. O administrador da plataforma consegue filtra os usuários cadastrados.
> O filtro pode ser por Nome, Telefone/Celular e E-mail.
> O administrador acessa "Reservas" e um front com estes campos estará disponível para fazer a consulta.

2. Administradores não tem a função de fazer a reserva e não ocupam espaço na plateia. 

3. O administrador da plataforma pode bloquear os usuários por qualquer motivo, por exemplo, aqueles que marcaram a visita e não compareceram.

# [Funcionalidades]({{ site.baseurl }}/DevTeam/Projetos/CPO/Páginas-&-Funcionalidades.html)

O sistema possui: Cadastro de Usuários, Usuários Administradores, Agenda, Bloqueio, Impressão, Controle e Consulta de Usuários de Sistem.

# Desafios

- As pessoas se conscientizarem sobre o uso da tecnologia. Elas precisarão ter acesso a Internet e acessarem o website para fazerem um cadastramento.

- As pessoas terão acesso rápido a agenda, conseguirão fazer de forma autônomo. O atual processo exige um trabalho manual e atenção, pelo administrador do sistema para fazer a reserva.

- Usuários não cadastrados precisam ser orientados pelos administradores a fazerem o cadastro.

# Benefícios

- Elimina o processo de agendamento manual um a um.
- O usuários terão a confirmação
