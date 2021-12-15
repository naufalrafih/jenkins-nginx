FROM jenkins/jenkins:lts
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
COPY plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt
COPY casc.yaml /usr/local/casc.yaml
ENV CASC_JENKINS_CONFIG /usr/local/casc.yaml

USER root
RUN apt-get update
RUN apt-get install -y sshpass