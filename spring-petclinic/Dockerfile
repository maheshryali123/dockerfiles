FROM ubuntu:22.04
RUN apt update
RUN apt install maven git -y
RUN apt install openjdk-17-jdk -y
RUN git clone https://github.com/maheshryali123/spring-petclinic.git
WORKDIR spring-petclinic/
RUN mvn package
WORKDIR /spring-petclinic/target/
EXPOSE 8080
CMD [ "java", "-jar", "spring-petclinic-3.0.0-SNAPSHOT.jar"]
