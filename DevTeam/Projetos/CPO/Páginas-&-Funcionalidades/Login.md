---
title: "Login"
nav_order: 9
parent: "Páginas & Funcionalidades"
---

Permitir que os usuários acessem a agenda e façam uma reserva de forma autônoma. Antes de fazer uma reserva, a pessoa precisa estar cadastrada na Casa Plataforma de Oração.

Existe duas formas de cadastramento:

- **Login Gmail** > Selecionando a opção **Gmail**, sendo autorizada pelo Google via OAuth. Se o usuário não estiver cadastro na plataforma, será direcionado para a tela de "Registro" automaticamente. Os campos E-mail e Senha, estarão bloqueados neste cenário.

- **Login Credencial** > Digitando seu Email e Senha (credencial). Se o usuário não estiver cadastro na plataforma, um alerta será emito para ele se "Registrar". 

Para os dois cenários é necessário que o usuário se cadastre na plataforma. Este procedimento pode ser feito diretamente pelo botão "Registra".

Critério: Dado que o usuário se cadastrou na plataforma com seu @gmail.com e credencial própria, quando ele tentar logar pelo "Gmail", então não será permitido.

Critério: Dado que o usuário se cadastrou pelo Google (conta@gmail.com), a senha e autenticação a ser utilizada será do Google. Caso a pessoa tente logar usando e e-mail ou cadastrar um credencial, não será permitido.