FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD cls-apigateway-0.0.1-SNAPSHOT.jar cls-apigateway-0.0.1-SNAPSHOT.jar
RUN sh -c 'touch /cls-apigateway-0.0.1-SNAPSHOT.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /cls-apigateway-0.0.1-SNAPSHOT.jar" ]