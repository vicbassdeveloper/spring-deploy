ADD file:9893213a9ea238f53ac68d87a3cf2f05d86763688392e5ddb6a2c9b60d3550a6 in / 
 CMD ["/bin/bash"]
ENV JAVA_HOME=/usr/java/openjdk-17
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
ENV LANG=C.UTF-8
ENV JAVA_VERSION=17.0.2
CMD ["jshell"]
COPY ./target/spring-deploy-1.0.jar app.jar
EXPOSE map[8086/tcp:{}]
ENTRYPOINT ["java", "-jar", "app.jar"]
