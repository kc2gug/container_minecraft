FROM kc2gug/container_centos7_java:latest

RUN yum -y update && yum clean all && useradd -ms /bin/bash minecraft -d /minecraft/ 
COPY server.jar /minecraft/
COPY eula.txt /minecraft/


USER minecraft
WORKDIR /minecraft

ENTRYPOINT ["/bin/bash"]
##ENTRYPOINT ["/usr/bin/java -Xmx4098M -Xms4098M -jar /minecraft/server.jar nogui"]

