FROM jenkins/jenkins:2.345-alpine
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
COPY default-user.groovy /usr/share/jenkins/ref/init.groovy.d/
#COPY plugins.txt /usr/share/jenkins/plugins.txt
#RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/plugins.txt
COPY plugins/* /var/jenkins_home/plugins/
USER root
