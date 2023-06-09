FROM ubuntu:latest AS build
RUN apt-get update && apt-get install -y locales && rm -rf /var/lib/apt/lists/* \
	&& localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
ENV LANG en_US.utf8
RUN apt-get install openjdk-17-jdk
COPY "/home/alex/Documentos/EjerciciosOpenBootCamp/cursospring/Ejercicios101112/peticiones-ob/target/spring-deploy-1.0.jar" "app.jar"
EXPOSE 8086
ENTRYPOINT ["java","-jar","app.jar"]