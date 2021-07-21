## O Problema
A incorporadora Cyrela possui três braços a Cyrela, a Living e a Vivaz. Sendo que esta última não possui um aplicativo próprio. Como não possui documentação técnica e a equipe de desenvolvimento é enxuta, foi apresentado um problema, na área de assistência técnica, no qual consiste em como lidar com as ocorrências que por consequência acabam gerando os agendamentos.

## A Solução
Desenvolvimento de uma Web Api em .NET Core com uma abordagem em Code First Migrations, e o Entity Framework para a persistência dos dados em um banco de dados Postgresql.

Inicializa o banco de dados (necessário ter o docker e docker-compose instalados):

```console
docker-compose up -d
```

Instala as dependências do projeto:

```console
dotnet restore
```

Executa as migrações e o seed no banco de dados:

```console
dotnet ef database update
```

Inicia o servidor da aplicação:

```console
dotnet run
```
