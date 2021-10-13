## Dockerfile
installer docker avec le script : https://get.docker.com/

```curl -fsSL https://get.docker.com -o get-docker.sh```

```sh get-docker.sh```

### Builder l'image
```sudo docker build -t visagesanimesjs .```
### Docker run pour lancer le conteneur à base de l'image

```sudo docker run --name nomimage:version -d -p 8081:80 visagesanimesjs```
### accedrer à l'aplication via le navigateur
```@ip:8081``` 


## docker-compose
insatller docker-compose **for linux https://docs.docker.com/compose/install/
```sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose```
```sudo chmod +x /usr/local/bin/docker-compose```