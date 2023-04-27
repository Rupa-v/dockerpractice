FROM ubuntu:22.04
LABEL author="Rupa" organization="QT" project="jenkinsfile"
RUN apt update 
RUN apt install openjdk-11-jdk maven -y
RUN apt install curl -y
RUN curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
RUN echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
RUN apt update && apt install jenkins -y  
EXPOSE 8080
CMD [ "/usr/bin/jenkins" ]