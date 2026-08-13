---
title: "API MP4 to FLAC"
nav_order: 2
parent: "Arquivos"
---

### Resumo do Código `API_MP4_to_FLAC.py`

---

#### Importações de Bibliotecas

- `from moviepy.editor import *`: Importa todos os métodos e classes do módulo `moviepy.editor`, utilizado para manipular arquivos de áudio e vídeo.
- `import os`: Importa o módulo `os`, que fornece uma maneira de usar funcionalidades dependentes do sistema operacional, como ler ou escrever em arquivos.

#### Funções

1. **`list_mp4_files(directory)`**

    - **Objetivo**: Listar todos os arquivos `.mp4` em um diretório especificado.
    - **Entrada**: Caminho do diretório onde os arquivos `.mp4` estão armazenados.
    - **Retorno**: Uma lista contendo os nomes dos arquivos `.mp4`.
    - **Método**: Usa o método `os.listdir()` para listar todos os arquivos no diretório e a compreensão de lista para filtrar apenas arquivos com a extensão `.mp4`.

2. **`convert_mp4_to_flac(mp4_path, flac_path)`**

    - **Objetivo**: Converter um arquivo de áudio em formato `.mp4` para `.flac`.
    - **Entrada**: Caminho do arquivo `.mp4` e o caminho onde o arquivo `.flac` deve ser salvo.
    - **Método**: Utiliza o método `AudioFileClip` da biblioteca `moviepy.editor` para ler o arquivo `.mp4` e o método `write_audiofile` para escrever o arquivo `.flac`.
  
#### Fluxo Principal (`__main__`)

- Define os caminhos dos diretórios onde os arquivos `.mp4` e `.flac` serão armazenados.
- Chama a função `list_mp4_files()` para obter uma lista de todos os arquivos `.mp4` no diretório especificado.
- Percorre cada arquivo `.mp4` e:
    - Constrói o caminho completo para o arquivo `.mp4` e o arquivo `.flac` resultante.
    - Chama a fu