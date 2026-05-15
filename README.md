# Exercício 9.4 - Nuvem

## API RESTful com Flask

Este projeto consiste em uma API RESTful desenvolvida utilizando Flask e hospedada na Microsoft Azure utilizando Azure App Service.

## Tecnologias utilizadas

* Python
* Flask
* Gunicorn
* GitHub
* Azure App Service
* GitHub Actions (CI/CD)
* Postman

## Funcionalidades da API

A API permite realizar operações CRUD de tarefas:

* Listar tarefas
* Buscar tarefa por ID
* Criar tarefa
* Atualizar tarefa
* Remover tarefa

## Rotas disponíveis

### Página inicial

GET /

Retorna mensagem de funcionamento da API.

### Listar tarefas

GET /tarefas

### Buscar tarefa por ID

GET /tarefas/<id>

### Criar tarefa

POST /tarefas

Exemplo JSON:

{
"titulo": "Nova tarefa",
"concluida": false
}

### Atualizar tarefa

PUT /tarefas/<id>

Exemplo JSON:

{
"titulo": "Tarefa atualizada",
"concluida": true
}

### Remover tarefa

DELETE /tarefas/<id>

## Como executar localmente

Instalar dependências:

pip install -r requirements.txt

Executar aplicação:

python app.py

## Deploy na Azure

A aplicação foi publicada utilizando Azure App Service no plano Free F1.

O deploy automático foi configurado utilizando GitHub Actions (CI/CD).
