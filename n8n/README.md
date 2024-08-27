# Workflows do n8n

Este repositório contém uma coleção de workflows exportados do n8n que podem ser facilmente importados e utilizados em sua própria instância do n8n. No final deste documento, você encontrará instruções sobre como executar o Docker Compose em sistemas Windows, Linux e Mac.

## Índice
1. [Descrição dos Workflows](#descrição-dos-workflows)
2. [Como Importar Workflows no n8n](#como-importar-workflows-no-n8n)
3. [Executando o n8n com Docker Compose](#executando-o-n8n-com-docker-compose)
4. [Contribuições](#contribuições)

## Descrição dos Workflows

| Arquivo                                                                     | Descrição                                                                                                          |
|-----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| `Cafe Tech - Evento 2 - API Simples.json`                                  | Exemplo de como construir uma API simples utilizando n8n. A API lê feeds RSS de múltiplos portais de notícia e gera uma resposta JSON consolidada. |
| `Cafe Tech - Evento 2 - Chat Simples - Completo.json`                      | Exemplo de chat web, utilizando como LLM OpenAI. O chat sabe especificamente responder perguntas de nosso evento Café Tech.                   |
| `Cafe Tech - Evento 2 - Clínica Médica - Agendamento de Exames.json`       | Sub-workflow do Clínica Médica - Agente Virtual - Completo.json, responsável pela integração com o Google Calendar.                          |
| `Cafe Tech - Evento 2 - Clínica Médica - Agente Virtual - Completo.json`   | Workflow completo, que contempla o fluxo de atendimento de uma clínica médica, desde a coleta dos dados do paciente, a lista de exames até o agendamento dos exames em um Google Calendar. |
| `Cafe Tech - Evento 2 - Formulário.json`                                    | Exemplo de como criar um formulário simples e receber o post em um workflow.                                      |

## Como Importar Workflows no n8n

Para importar um workflow no n8n, siga os passos abaixo:

1. Acesse sua instância do n8n.
2. No painel lateral, clique em "Workflows".
3. Clique em "Importar" no canto superior direito.
4. Selecione o arquivo JSON do workflow que você deseja importar.
5. Clique em "Importar" novamente.

Após a importação, o workflow estará disponível na lista de workflows e pronto para ser editado e executado.

## Executando o n8n com Docker Compose

Você pode executar o n8n localmente usando o Docker Compose. Para isso, siga os passos abaixo dependendo do seu sistema operacional:

### Windows

1. Certifique-se de ter o Docker Desktop instalado e em execução.
2. Navegue até a pasta onde está o arquivo `docker-compose.yml`.
3. Abra o terminal (cmd ou PowerShell) e execute o seguinte comando:

   ```bash
   docker compose up
   ```

4. Acesse o n8n em [http://localhost:5678](http://localhost:5678).

*Se necessário, adicione um printscreen do terminal e da interface do Docker.*

### Linux

1. Certifique-se de ter o Docker e o Docker Compose instalados.
2. Navegue até o diretório onde está o `docker-compose.yml`.
3. Abra o terminal e execute o seguinte comando:

   ```bash
   sudo docker compose up
   ```

4. Acesse o n8n em [http://localhost:5678](http://localhost:5678).

*Caso necessário, insira uma imagem do terminal Linux e da interface do Docker.*

### Mac

1. Instale o Docker Desktop se ainda não tiver.
2. Navegue até a pasta com o arquivo `docker-compose.yml`.
3. Abra o terminal e execute:

   ```bash
   docker compose up
   ```

4. Acesse o n8n em [http://localhost:5678](http://localhost:5678).
