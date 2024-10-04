# Atividade 2: Docker Compose - Pós-Graduação em Engenharia de Dados

Este projeto é parte da disciplina de Engenharia de Dados da pós-graduação na Impacta. A atividade envolve a criação de um ambiente com Docker Compose que executa uma aplicação Flask simples balanceada com Nginx.


📄 Explicação dos Arquivos

Aqui estão os detalhes de cada arquivo e diretório presentes no repositório e suas funcionalidades:

- **Evidencia exec/**: Diretório contendo as evidências das execuções, como screenshots ou logs, que demonstram o funcionamento do projeto.

- **atividade_2/**: Diretório principal do projeto que contém todos os arquivos necessários para a execução da aplicação.

  - **venv/**: Ambiente virtual Python, que isola as dependências da aplicação para evitar conflitos com outras instalações no sistema.

  - **app.py**: Arquivo principal da aplicação Flask. Ele define uma rota simples que exibe o nome do servidor e o endereço IP quando acessada via navegador.

  - **Dockerfile**: Arquivo de configuração para o Docker que define como a imagem do contêiner será construída. Ele especifica a imagem base, as dependências necessárias, o diretório de trabalho, e o comando para iniciar a aplicação Flask.

  - **nginx.conf**: Arquivo de configuração do Nginx que define como o proxy reverso é configurado para balancear a carga entre as instâncias da aplicação Flask (web1 e web2).

  - **docker-compose.yml**: Arquivo de configuração do Docker Compose que orquestra os serviços `web1`, `web2` e `nginx`, permitindo que eles sejam executados em conjunto com suas respectivas configurações.

  - **requirements.txt**: Arquivo que lista todas as dependências Python necessárias para o projeto. Ele é utilizado pelo Docker e pelo ambiente virtual para instalar os pacotes requeridos pela aplicação.

