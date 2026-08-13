---
title: "API FLAC to CUTS.py"
nav_order: 1
parent: "Arquivos"
---

### Resumo Detalhado do Código `API_FLAC_to_CUTS.py`

#### Configurações Globais e Importações
- `import os`: Importa o módulo `os` para operações relacionadas ao sistema operacional.
- `from pydub import AudioSegment`: Importa `AudioSegment` da biblioteca `pydub` para manipulação de áudio.
- Define os caminhos para `ffmpeg` e `ffprobe`, que são necessários para a manipulação de áudio.

#### Funções

1. **`split_audio_into_segments(audio, segment_length_ms=120000)`**
    - **Objetivo**: Divide o áudio em segmentos de uma determinada duração em milissegundos.
    - **Parâmetros**: 
        - `audio`: O objeto de áudio a ser dividido.
        - `segment_length_ms`: O comprimento de cada segmento em milissegundos (padrão é 120000 ms ou 2 minutos).
    - **Retorno**: Retorna uma lista de segmentos de áudio.

2. **`save_segments_to_disk(segments, base_path)`**
    - **Objetivo**: Salva os segmentos de áudio no disco rígido.
    - **Parâmetros**:
        - `segments`: Lista de segmentos de áudio.
        - `base_path`: O caminho base para salvar os arquivos.
    - **Retorno**: Não retorna nada, mas salva os segmentos em arquivos `.flac`.

#### Fluxo Principal (`if __name__ == "__main__":`)
- Define os diretórios de entrada e saída.
- Itera sobre cada arquivo `.flac` no diretório de entrada:
    - Carrega o arquivo `.flac` como um objeto `AudioSegment`.
    - Divide o arquivo de áudio em segmentos de 2 minutos.
    - Salva os segmentos no disco rígido.

Essencialmente, esse script pega arquivos de áudio FLAC de um diretório de entrada, divide-os em segmentos e salva os segmentos em um diretório de saída. Isso é especialmente útil para contornar limitações de tamanho de arquivo e duração ao trabalhar com APIs de transcrição ou outros serviços de processamento de áudio.