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

### Após o processo para incluir as dependências na sua aplicação:

Em application.properties, adicione:

        spring.datasource.url=jdbc:mysql://localhost:3306/name
        spring.datasource.username=root
        spring.datasource.password=


#### Rodar novamente ;) 