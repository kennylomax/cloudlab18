#FROM jenkins/jenkins:2.249.2-jdk11
FROM jenkinsci/blueocean:1.24.4

COPY docker-resources/plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt

COPY docker-resources/jenkins.yaml /usr/share/jenkins/ref/jenkins.yaml
#COPY docker-resources/sonarqubeGoodCodeJob.xml /usr/share/jenkins/ref/jobs/sonarqube-good-code/config.xml
#COPY docker-resources/sonarqubeBadCodeJob.xml /usr/share/jenkins/ref/jobs/sonarqube-bad-code/config.xml
#COPY docker-resources/sonarqubeSlowFast.xml /usr/share/jenkins/ref/jobs/sonarqube-slowfast/config.xml

COPY seedJob.xml /usr/share/jenkins/ref/jobs/seed-job/config.xml
#COPY createJobs.groovy /var/jenkins_home/jobs/seed-job/workspace/createJobs.groovy

ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
USER root