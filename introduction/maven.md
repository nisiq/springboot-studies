
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
