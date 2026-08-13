---
title: "Landing Page"
nav_order: 7
parent: "Páginas & Funcionalidades"
---


Representa a "página de entrada" para os usuários, fornecendo a visão para acessar os links:

- Site (Agendamento)
- YouTube (Vídeos)
- Telegram (Chat)
- Spotify (Áudios)

Para tornar a "Landing Page" facilmente editável sem necessidade de acessar um banco de dados, e para facilitar o entendimento de onde fazer alterações, podemos criar uma estrutura baseada em constantes/configurações.

# 1. Organize as Configurações:

Em sua estrutura de projeto, crie um arquivo chamado `config.ts` (ou algo similar) dentro do diretório `src`.

No arquivo `config.ts`, você pode criar uma estrutura de dados para armazenar as informações da "Landing Page". 


# 2. Consuma as Configurações no Componente:

No componente `App.tsx` (ou onde quer que você esteja renderizando a "Landing Page"), importe e use o arquivo de configuração.


### Vantagens:

1. **Facilidade de Edição**: Qualquer pessoa com um conhecimento mínimo sobre a estrutura do projeto pode ir diretamente ao arquivo `config.ts` e fazer alterações nos links, URLs e logotipos, sem ter que mexer no código principal ou no banco de dados.

2. **Centralização**: Todas as configurações relacionadas à "Landing Page" estão em um único lugar, tornando mais fácil para os desenvolvedores entenderem e modificarem.

3. **Flexibilidade**: Caso no futuro você decida mover essas configurações para um banco de dados ou outro meio de armazenamento, a separação em um arquivo de configuração tornará essa transição mais fácil.
