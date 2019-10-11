FROM maven:3.6.2-jdk-11

RUN adduser --quiet jenkins && \
	usermod -aG sudo jenkins

ADD settings.xml /home/jenkins/.m2/

RUN chown -R jenkins:jenkins /home/jenkins/.m2/

VOLUME ["/var/jenkins_home/dep"]