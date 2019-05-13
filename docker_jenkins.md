* Use docker to run jenkins in a container (command-line is from the jenkins official image on dockerhub)

```
    docker run -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home --name jenkins jenkins/jenkins:lts
```

* Get the admin password

```
    docker exec -it jenkins cat /var/jenkins_home/secrets/initialAdminPassword
```
