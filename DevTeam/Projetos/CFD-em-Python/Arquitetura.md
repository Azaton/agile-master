---
title: "Arquitetura"
nav_order: 1
parent: "CFD em Python"
---

# Bibliotecas Utilizadas

- Sqlite3: Utilizada para interagir com bancos de dados SQLite.
- Flask: Estrutura web em Python usada para criar aplicativos web.
- Seaborn: Biblioteca de visualização de dados baseada em Matplotlib, que fornece uma interface de alto nível para criação de gráficos estatísticos.
- Numpy: Biblioteca numérica em Python que fornece suporte para arrays e funções matemáticas.
- Matplotlib.pyplot: Biblioteca de plotagem em Python que permite criar gráficos e visualizações.
- Os: Fornece funcionalidades dependentes do sistema operacional, como manipulação de arquivos e diretórios.

# Funções & Rotas

- render_template e send_from_directory: Essas funções são fornecidas pelo Flask para renderizar modelos de template HTML e enviar arquivos estáticos.
- serve_chart(filename): Esta função é um manipulador de rota que serve arquivos estáticos do diretório "static". É usado para fornecer a imagem do gráfico gerado.
- show_cfd_chart(): Esta função é um manipulador de rota que executa a lógica principal para criar o gráfico CFD.

1. Conecta-se ao banco de dados SQLite usando a biblioteca sqlite3.
1. Executa uma consulta SQL para selecionar todos os dados da tabela "TB_CFD".
1. Separa os dados em listas para plotagem do gráfico.
1. Cria o gráfico CFD usando a biblioteca seaborn e matplotlib.pyplot.
1. Salva o gráfico em um arquivo temporário no diretório "static".
1. Renderiza o template HTML "chart.html" passando o caminho do gráfico como parâmetro.

# Integração (Código)

- A aplicação Flask é criada através da instância Flask(__name__).
- O diretório "static" é definido usando a biblioteca os para fornecer o caminho absoluto para o diretório.
- Duas rotas são definidas usando o decorador @app.route para servir a imagem do gráfico e exibir o gráfico.
- Dentro da função show_cfd_chart(), o banco de dados é conectado, a consulta SQL é executada, os dados são processados e o gráfico é criado.