# Module 3

Esse repositorio é criado com o intuito de disponibilizar um acesso facilitado ao banco de dados que usaremos nessa mentoria. Para isso é necessario ter docker e docker compose instalado na máquina.

Dentro de nosso docker-compose.yml iniciamos um serviço de banco de dados postgres. Para iniciar use: docker-compose -f docker-compose.yml up -d ou docker-compose up -d. Isso baixara as imagens necessárias e começara a rodar o banco de dados no background

Para acessar o banco de dados faça:

```
docker exec -it node_db bash

psql -U postgres
```

A primeira linha diz que você quer entrar no bash do container e a segunda você entra dentro do banco de dados

Agora faça:

```
\l -> Verá todos os bancos
\d -> Verá todas as relações

\connect node -> Entrar dentro do banco de dados node
```

Agora com acesso ao banco de dados você pode realizar suas querys.
