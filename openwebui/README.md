# OpenWebUI

OpenWebUI é uma ferramenta poderosa projetada para orquestrar múltiplos Modelos de Linguagem (LLMs) de forma eficiente e intuitiva. Com uma interface amigável, OpenWebUI permite que você interaja com diferentes modelos de linguagem, otimizando a criação de produtos digitais que utilizam inteligência artificial.

## Pré-requisitos

Antes de começar, verifique se você possui o Docker e o Docker Compose instalados em sua máquina. Você pode baixar o Docker [aqui](https://docs.docker.com/get-docker/) e o Docker Compose [aqui](https://docs.docker.com/compose/install/).

## Como Executar

Para executar o OpenWebUI e o Ollama, siga as etapas abaixo:

1. **Executar o Docker Compose**

   Com o terminal posicionado no diretório do repositório clonado, execute o seguinte comando:

   ```bash
   docker compose up -d
   ```

   Este comando irá iniciar os serviços definidos no arquivo `docker-compose.yml`, incluindo o OpenWebUI e o Ollama.

2. **Acessar a Interface Web**

   Após a execução do Docker Compose, acesse a interface do OpenWebUI abrindo seu navegador e indo para a seguinte URL:

   ```
   http://localhost:3000/
   ```

## Estrutura do Projeto

### Docker Compose

O arquivo `docker-compose.yml` contém a configuração necessária para orquestrar os contêineres do OpenWebUI e do Ollama. Ele define as imagens, as portas a serem expostas e quaisquer dependências necessárias.

### Dependências

O OpenWebUI trabalha em conjunto com o Ollama, que permite a implementação e o uso dos modelos de linguagem. O Docker Compose garante que todas as dependências sejam estabelecidas corretamente.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests para melhorar o projeto.
