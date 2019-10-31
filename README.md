﻿### Central de Erros
### Objetivo
Em projetos modernos é cada vez mais comum o uso de arquiteturas baseadas em serviços ou microsserviços. Nestes ambientes complexos, erros podem surgir em diferentes camadas da aplicação (backend, frontend, mobile, desktop) e mesmo em serviços distintos. Desta forma, é muito importante que os desenvolvedores possam centralizar todos os registros de erros em um local, de onde podem monitorar e tomar decisões mais acertadas. Neste projeto vamos implementar um sistema para centralizar registros de erros de aplicações.

A arquitetura do projeto é formada por:

## Backend - API
criar endpoints para serem usados pelo frontend da aplicação
criar um endpoint que será usado para gravar os logs de erro em um banco de dados relacional
a API deve ser segura, permitindo acesso apenas com um token de autenticação válido
## Frontend
deve implementar as funcionalidades apresentadas nos wireframes
deve ser acessada adequadamente tanto por navegadores desktop quanto mobile
deve consumir a API do produto
desenvolvida na forma de uma Single Page Application
## Observações
Se a aceleração tiver ênfase no backend (Java, Python, C#, Go, PHP, etc) a equipe deve obrigatoriamente implementar a API. A implementação do frontend é considerado um bônus importante
Se a aceleração tiver ênfase em frontend (React, Vue, Angular, etc) a equipe deve obrigatoriamente implementar o frontend da aplicação e o backend pode ser substituido por uma aplicação mock. A implementação da API é considerado um bônus importante
## Wireframes
Os wireframes a seguir servem para demonstrar as funcionalidades básicas da aplicação.

https://www.codenation.dev/private-journey/java-florianopolis-1/challenge/central-erros

## Git Guidelines

Todo commit deve ter um comentário que possua o mínimo de informações sobre as modificações feitas,
lembre-se de dar um `git pull` na branch master antes de criar uma nova branch ou
dar um `git push` na master.

## Ferramentas
* XMind;
* BR Modelo;
* Trello para gerenciamento de projetos;
* Postman
* Angular

## Solução

### Classe Log
Devemos criar um pacote utilitário com métodos que retornem s mensagens de log para cada caso de uso:
Backend, FrontEnd e Mobile e Desktop, portanto ela deve ter métodos static que implementem a geração de Logs.

A classe de Log pode ser abstract para que as classes que utilizarem o Log implementem os métodos de Log de forma
personalizada.

* Entidade,
* Timestamp,
* Descrição,

## Lista de Tarefas
1. Criar a modelagem conceitual do BD;
2. Criar as entidades em java com base na modelagem feita;
3. Criar Repository e Service;
4. Definir as rotas (controller);
5. Testar as rotas com Postman;
6. Autenticação e Autorização;
7. Criar as telas de front-end:
7.1. Cadastro de Usuário;
7.2. Login;
7.3. Consulta de erros;
7.4. (Opcional) Arquivo com erros que irão popular o banco de dados em x minutos;
8. Deploy (Heroku?)
9. Testes (Opcional)
10. Slides da apresentação;
