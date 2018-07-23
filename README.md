# jenkinsindocker
https://github.com/jenkinsci/docker

Run local jenkins 

https://github.com/jenkinsci/docker

docker run -d -v jenkins_home:/var/jenkins_home -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts

Without slave/jnlp port open and in detached mode

docker run -d -v jenkins_home:/var/jenkins_home -p 8080:8080  jenkins/jenkins:lts

to enter into bash on a running container

docker exec -i -t 77f94fd80dd5 /bin/bash

locate the initial password

cd /var/jenkins_home/secret
cat initialAdminPassword

Browse jenkins to proceed with inital setup
http://localhost:8080/


http://localhost:8080/view/all/
