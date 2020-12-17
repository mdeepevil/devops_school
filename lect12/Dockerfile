FROM maven:3.6.3-jdk-8
RUN apt-get update \
    apt-get upgrade -y \
    apt-get install git -y
RUN git clone https://github.com/mdeepevil/lect12-project.git
RUN mvn package -f /lect12-project/pom.xml
RUN cp /lect12-project/target/*.war /home/app/data