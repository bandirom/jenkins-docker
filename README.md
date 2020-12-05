# jenkins-docker
### Autorun Jenkins in docker using docker-compose

    docker-compose up -d 
    
## Copy secret key:

    $ docker-compose exec jenkins sh

    $ cat /var/jenkins_home/secrets/initialAdminPassword

    
