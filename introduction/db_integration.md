# Integração Mysql com a aplicação

### Dependencias Necessárias
- Validation

    Responsável pela validação de campos da nossa requisição

- MySQL Driver

    Integração com o banco de dados

- FlyWay Migration

    Controlar migrações do banco de dados

- Spring Data JPA

    Facilitar a criação de entidades, integração de entidades...

### Após o processo para incluir as dependências na aplicação:

Em application.properties, adicione:

        spring.datasource.url=jdbc:mysql://localhost:3306/name
        spring.datasource.username=root
        spring.datasource.password=


#### Rodar novamente para testar ;) 


## Criação de Tabelas
Utiliza-se o FlyWay Migration

- Não executar migration com o projeto rodando
- Extensão pra editar diretamente na IDE, 


src/main/resources/db/migration
deve ser padrão: "V1__create-table-remedios.sql" .sql!!!!!!

exemplo:
        create table remedios(

            id bigint not null auto_increment,
            nome varchar(100) not null,
            via varchar(100) not null,
            lote varchar(100) not null,
            quantidade varchar (100) not null,
            validade varchar(100) not null,
            laboratorio varchar(100) not null,

            primary key(id)
            );