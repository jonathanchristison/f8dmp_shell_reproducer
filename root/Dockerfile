from ${docker.image.from}

ENV HOME /home/jenkins

RUN export PATH="$PATH:/home/jenkins/da-cli/:/home/jenkins/maven/apache-maven-${MAVEN_VERSION}/bin"

RUN groupadd -g 1001 jenkins
RUN useradd -u 1001 -d $HOME -g jenkins jenkins


USER jenkins

WORKDIR /home/jenkins/bin
ENTRYPOINT ["/bin/bash", "-l", "-c"]
