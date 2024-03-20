
# Maven

Ferramenta de gerenciamento de dependências que foi feita em Java para auxiliar nos códigos feitos nesta linguagem.

Este modelo organiza todas as informações do projeto em um único arquivo: o pom.xml.

Ao desenvolver um projeto de programação temos que utilizar, muitas vezes, bibliotecas externas ao código feito para conseguir utilizar certas funcionalidades. Geralmente é feito o download da biblioteca e em seguida a importação dela no projeto.

Porém, a depender da complexidade do projeto, acaba sendo necessário o uso de diversas bibliotecas, que podem vir a ter problema na versão e/ou compatibilidade com o código; isso pensado em um projeto grande, passa a ser inviável realizar a importação e verificação de cada biblioteca manualmente. E assim, entra a importância de utilizar o Maven.

Conforme dependências são requisitadas, o POM é atualizado. O projeto Maven pode possuir módulos e cada módulo pode ter seu respectivo POM sem perder a organização e hierarquia do projeto principal.

# Demonstração pom.xml
https://www.alura.com.br/artigos/assets/conhecendo-melhor-maven/imagem4.jpg



## Instalando o Maven no Windows

https://maven.apache.org/download.cgi > Binary zip archive - apache-maven-3.9.6-bin.zip


- Extrair Arquivos
- Sugestão: Renomeie a pasta para "Maven"
- Recorte ela e cole em: Disco Local (C:) > Arquivos de Programas

Caminho deve estar similar a isso: 

- Este Computador > Disco Local (C:) > Arquivos de Programas > Maven > apache-maven-3.9.6

- Copie este endereço e vá até a vá até Editar Variáveis de Ambiente

- Crie uma nova Variável do SISTEMA:

        nome da variável: MAVEN_HOME

        valor da variável: caminho copiado anteriormente
        
        ok

- Após isso, abrir o path localizado também em variávies do sistema e clicar em "novo"

        na nova linha coloque: "%MAVEN_HOME%/bin"
        ok > ok > ok

# Teste 
- Abra o CMD e digite

        mvn -v

## Referência

 - [Conhecendo Melhor o Maven](https://www.alura.com.br/artigos/conhecendo-melhor-maven)

 - [Instalação Maven](https://youtu.be/ggQa14MC2s0?si=Lusg8e9AEhSAMvfP)

