FROM ubuntu:latest

WORKDIR /dir_to_runjavaapp

COPY . /dir_to_runjavaapp

RUN sudo apt update
RUN sudo apt install -y openjdk-17-jdk
RUN sudo apt install -y openjdk-17-jre

CMD ["javac", "app.java"]
CMD ["java", "Main"]
