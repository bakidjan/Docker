## Dockerfile
installer docker avec le script _https://get.docker.com/
``curl -fsSL https://get.docker.com -o get-docker.sh``
``sh get-docker.sh``

### Faire une build de l'image
```
sudo docker build -t visagesanimesjs .
```
### Docker run pour lancer le conteneur à base de l'image
