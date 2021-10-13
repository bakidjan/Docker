## Dockerfile
installer docker avec le script : https://get.docker.com/

```curl -fsSL https://get.docker.com -o get-docker.sh```

```sh get-docker.sh```

### Builder l'image
```
sudo docker build -t visagesanimesjs .
```
### Docker run pour lancer le conteneur à base de l'image

```sudo docker run --name nomimage:version -d -p 8081:80 visagesanimesjs```
