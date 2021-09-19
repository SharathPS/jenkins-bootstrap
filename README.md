# jenkins-bootstrap
casc.yaml: configures jenkins
plugins.txt: list of plugins to be installed

# docker image
### Build 
docker build -t jenkins:jcasc .
### Run container
docker run --name jenkins --rm -p 8080:8080 --env JENKINS_ADMIN_ID=admin --env JENKINS_ADMIN_PASSWORD=password jenkins:jcasc

Note: Once docker run is quit image gets deleted (rm)
