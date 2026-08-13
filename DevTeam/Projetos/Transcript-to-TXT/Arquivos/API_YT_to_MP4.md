---
title: "API YT to MP4"
nav_order: 4
parent: "Arquivos"
---

### Arquivo: `API_YT_to_MP4.py` (versão simplificada)

#### Importações
- `from pytube import YouTube`: Importa o módulo `YouTube` da biblioteca `pytube` para baixar vídeos do YouTube.
- `import os`: Importa o módulo `os` para manipulação de variáveis de ambiente e caminhos de arquivos.

#### Configurações de Ambiente
- `os.environ["GOOGLE_APPLICATION_CREDENTIALS"]`: Define a variável de ambiente para as credenciais do Google Cloud. Embora essa parte não seja utilizada neste script simplificado, ela está presente caso você precise de recursos do Google Cloud em outras partes do projeto.

#### Funções

1. `safe_file_name(file_name)`:  
    - **Objetivo**: Recebe um nome de arquivo e retorna uma versão "segura" desse nome, removendo caracteres especiais e espaços.
    - **Parâmetros**: `file_name` é o nome original do arquivo.
    - **Retorno**: Retorna um nome de arquivo "seguro".

2. `download_youtube_audio(url, path)`:  
    - **Objetivo**: Baixa o áudio de um vídeo do YouTube e o salva como um arquivo MP4.
    - **Parâmetros**: `url` é o URL do vídeo do YouTube, e `path` é o diretório onde o arquivo de áudio será salvo.
    - **Retorno**: Retorna o caminho completo do arquivo de áudio baixado e o título do vídeo.

#### Execução do Script

- `if __name__ == "__main__":`: Este bloco de código é executado quando o script é iniciado.
    - Define o `url` do vídeo do YouTube e o `download_path` onde o arquivo de áudio será salvo.
    - Chama a função `download_youtube_audio` para baixar o áudio do vídeo do YouTube.