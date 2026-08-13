---
title: "Upload Manual para o Google Storage"
nav_order: 5
parent: "Arquivos"
---

### Resumo Detalhado do Item 4: Upload Manual para o Google Cloud Storage

#### Etapas Preliminares
- **Conta de Faturamento**: É necessário ter uma conta de faturamento ativa no Google Cloud para acessar serviços pagos, como o Google Cloud Storage.
  
- **Criação de um Projeto**: Um novo projeto no Google Cloud Platform (GCP) precisa ser criado ou um existente selecionado para abrigar o serviço de armazenamento.

- **Criação do Serviço e Chave JSON**: 
  - É preciso criar um serviço associado ao projeto que tenha as permissões adequadas para acessar o Google Cloud Storage.
  - Uma vez que o serviço é criado, uma chave JSON é gerada. Essa chave será usada para autenticar o acesso programático ao Google Cloud Storage.

- **Configuração de Faturamento (Billing)**:
  - Se ainda não estiver configurado, você precisará associar uma forma de pagamento ao seu projeto. Isso permitirá que você pague pelos recursos consumidos pelo armazenamento.

#### Upload de Arquivos
- **Acessar a Interface Web do Google Cloud Storage**: Faça login na console do Google Cloud e navegue até o Google Cloud Storage.

- **Criar ou Acessar um Bucket**: Se ainda não existir um 'bucket', crie um. Escolha as configurações apropriadas, como classe de armazenamento, localização e controles de acesso.

- **Fazer Upload dos Arquivos**:
  - Navegue até o 'bucket' apropriado e utilize a opção de upload para fazer o upload manual dos arquivos FLAC segmentados.
  - Certifique-se de que os arquivos foram carregados com sucesso, visualizando-os na lista de objetos no bucket.

#### Notas
- **Limite de Tamanho e Duração**: O upload manual para o Google Cloud Storage é útil para contornar as limitações de tamanho de arquivo e de duração que você poderia enfrentar se estivesse fazendo upload direto para uma API, como o Google Speech-to-Text.

- **Segurança**: Mantenha sua chave JSON em um local seguro e nunca a exponha publicamente. Ela dá acesso aos seus recursos no Google Cloud, incluindo o armazenamento.

Este item detalha como armazenar manualmente os segmentos de áudio FLAC no Google Cloud Storage, para que eles possam ser acessados posteriormente para transcrição ou qualquer outra análise.