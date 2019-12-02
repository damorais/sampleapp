# Algumas instruções sobre o presente projeto

- Hot reloading depende do Java 1.8 (Tanto no gradle quanto na execução atraves do gradlew)
- Comandos:
    - ./gradlew -t build -> Monitora o classpath por alterações e compila se algo for alterado
    - ./gradlew run -> Executa a aplicação em modo de desenvolvimento
    
- Feito o upgrade da aplicação para o gradle 5.6.4
- Para executar usando o Docker:
    - ./gradlew build
    - docker build -t sampleapp .
    - docker run -m512M --cpus 2 -it -p 8080:8080 --rm sampleapp
    - Referência: https://ktor.io/quickstart/quickstart/docker.html