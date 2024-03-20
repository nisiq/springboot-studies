
# Criando Projeto com Springboot
Após a configuração do Maven...

----

# Spring Initializr
https://start.spring.io/


Ferramenta que fornece uma interface web bem simples para o usuário. Podendo gerar seu projeto a partir de uma estrutura de configurações pré-moldadas. São configurações de versões do java/spring boot, grupo/nome do projeto, série de lista de dependências e etc.

----

# Exemplo de configs
- Project: Maven
- Language: Java
- SpringBoot: 3.1.9
- Project Metadata:

        Group: com.remedios.nicole

        Artifact: Crud

        Name: Crud

        Description: Crud project for Spring Boot

        Package name: com.remedios.nicole

        Packaging: Jar
        
        Java: 17

- Dependencies 

        Spring Web

        Lombok
        
        Spring Boot DevTools

- Generate
----
# Após Download...

- Extrair a pasta
- Abrir no IntelliJ IDEA
- Rodar CrudApplication para iniciar a aplicação :)
- Após iniciada....... Acesse http://localhost:8081/ ou http://localhost:8080/
- Está ok:

        ""Whitelabel Error Page
        This application has no explicit mapping for /error, so
        you are seeing  this as a fallback....""

----
# Possíveis Erros:

        "Web server failed to start. Port 8080 was already in use.
        Action:
        Identify and stop the process that's listening on port 8080 or
        configure this application to listen on another port."
    
    
#### Solução: 

        em application.properties, adicionar a seguinte linha:
        --server.port=8081

----

        "Sei lá o que proxy"

 #### Solução: 
        COMPARTILHADO\PROVISÓRIO\Programas\Arquivos de Configuração\Arquivo de Configuração do MAVEN


---


# Hello World SpringBoot
Criar pasta Controllers.........

```
package com.remedios.nicole.controllers;

    import org.springframework.web.bind.annotation.GetMapping;
    import org.springframework.web.bind.annotation.RequestMapping;
    import org.springframework.web.bind.annotation.RestController;

    @RestController
    @RequestMapping("/hello")
    public class HelloWorld {
        @GetMapping
        public String helloWorld() {
            return "Hello World";
        }
    }
```
Rodar novamente CrudApplication e acessar http://localhost:8081/hello