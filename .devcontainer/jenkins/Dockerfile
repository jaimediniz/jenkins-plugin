FROM jenkins/jenkins:lts-jdk17

COPY --chown=jenkins:jenkins plugins.txt /tmp/plugins/plugins.txt
RUN jenkins-plugin-cli -f /tmp/plugins/plugins.txt
EXPOSE 8080
