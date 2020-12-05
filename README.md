# jenkins-docker
### Autorun Jenkins in docker using docker-compose
#### Dev version:
    docker-compose up -d --build
#### Prod version with SSL certificates
*Open the file docker/nginx-proxy/env/.env and change domain name

    VIRTUAL_HOST=jenkins.domain.com
    LETSENCRYPT_HOST=jenkins.domain.com
    
#### Run the command on your public server
    docker-compose -f prod.yml up -d --build
    
    
### Logs:
    docker-compose -f prod.yml logs -f
    
## Copy secret key:

    $ docker-compose exec jenkins sh

    $ cat /var/jenkins_home/secrets/initialAdminPassword

   