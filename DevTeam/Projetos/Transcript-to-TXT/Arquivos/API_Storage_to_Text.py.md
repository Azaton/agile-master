---
title: "API Storage to Text.py"
nav_order: 3
parent: "Arquivos"
---

Neste último código, `API_Storage_to_Text.py`, estamos realizando a transcrição de áudios armazenados no Google Cloud Storage, convertendo-os em arquivos de texto. 

### Importações e Configurações Iniciais
- `from google.cloud import storage, speech_v1p1beta1 as speech`: Importa as bibliotecas para interagir com o Google Cloud Storage e o Google Speech-to-Text.
- `import os`: Importa a biblioteca os para manipular variáveis de ambiente e caminhos de arquivos.
- `os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "D:\\DevOps\\Projetos\\API\\API_YT-WAV-TXT\\Chaves\\projeto-speech-398420-48b8f38561a7.json"`: Define a localização da chave de autenticação do Google Cloud.

### Definição de Parâmetros
- `bucket_name`, `folder_name`, `txt_dir`: Define o nome do bucket, o nome da pasta dentro do bucket e o diretório onde os arquivos de texto serão salvos, respectivamente.

### Inicialização de Clientes
- `storage_client = storage.Client()`: Inicializa o cliente do Google Cloud Storage.
- `bucket = storage_client.get_bucket(bucket_name)`: Obtém o bucket especificado.

### Listagem de Arquivos
- `blobs = bucket.list_blobs(prefix=folder_name)`: Lista todos os arquivos dentro da pasta especificada (`folder_name`) no bucket.

### Função de Transcrição (`transcribe_audio`)
1. `client = speech.SpeechClient()`: Inicializa o cliente do Google Speech-to-Text.
2. `audio = speech.RecognitionAudio(uri=file_path)`: Define o URI do arquivo de áudio a ser transcrito.
3. `config = speech.RecognitionConfig(...)`: Configura os parâmetros para a transcrição, incluindo o tipo de codificação, a taxa de amostragem, o idioma e o número de canais de áudio.
4. `operation = client.long_running_recognize(...)`: Inicia a operação de transcrição, que é uma tarefa demorada.
5. `response = operation.result(...)`: Obtém o resultado da transcrição.
6. `txt_file_path = os.path.join(...)`: Define o caminho onde o arquivo de texto será salvo.
7. `with open(txt_file_path, "w") as txt_file: ...`: Salva a transcrição em um arquivo de texto.

### Loop Principal
- O loop `for blob in blobs:` percorre todos os arquivos listados na pasta do bucket. Se o arquivo termina com ".flac", a função `transcribe_audio` é chamada para processar esse arquivo.

Essencialmente, o código automatiza o processo de pegar arquivos de áudio do Google Cloud Storage, transcrevê-los e então salvar as transcrições em arquivos de texto no sistema local.