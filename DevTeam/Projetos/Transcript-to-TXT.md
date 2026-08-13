---
title: "Transcript to TXT"
nav_order: 4
parent: "Projetos"
has_children: true
---

O sistema foi construído pelos seguintes programas (arquivos):

---

### 1. `API_YT_to_MP4.py`

- **Objetivo**: Baixa o áudio de um vídeo do YouTube e salva como um arquivo MP4.
- **Método**: Utiliza uma biblioteca, provavelmente `pytube`, para fazer o download do áudio.
- **Desafios**: O Google Speech-to-Text não suporta arquivos MP4 diretamente. A conversão para um formato suportado como FLAC ou WAV é necessária.
- **Nota**: A escolha do MP4 é feita para evitar problemas de tempo de requisição e limitações que podem ocorrer com outros formatos como WAV.

### 2. `API_MP4_to_FLAC.py`

- **Objetivo**: Converte o arquivo de áudio baixado de MP4 para FLAC.
- **Método**: Utiliza a biblioteca `pydub` para realizar a conversão.
- **Nota**: A conversão para FLAC mantém a qualidade do áudio e satisfaz os requisitos do Google Speech-to-Text.

### 3. `API_FLAC_to_CUTS.py`

- **Objetivo**: Divide o arquivo FLAC em vários segmentos menores, com duração especificada em milissegundos.
- **Método**: Utiliza as bibliotecas `pydub` e `os` para realizar a divisão dos arquivos.
- **Nota**: A divisão facilita a análise subsequente e ajuda a contornar as limitações de tamanho e duração da Google Speech-to-Text API.

### 4. Upload manual para o Google Cloud Storage

- **Objetivo**: Armazenar arquivos FLAC divididos para posterior transcrição.
- **Método**: Feito manualmente através da interface web do Google Cloud Storage.
- **Nota**: O armazenamento no Google Cloud Storage permite contornar as limitações de tamanho e duração impostas pela Google Speech-to-Text API.

### 5. `API_Storage_to_Text.py`

- **Objetivo**: Transcreve os arquivos de áudio FLAC armazenados no Google Cloud Storage para texto.
- **Método**: Utiliza a Google Speech-to-Text API para realizar a transcrição.
- **Nota**: A transcrição é feita diretamente a partir dos arquivos armazenados no Google Cloud Storage, evitando as limitações de tamanho e duração associadas ao envio direto de arquivos para a API.
