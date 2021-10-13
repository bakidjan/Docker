# IaC avec docker-compose
- Déployer le logiciel odoo à l'aide de docker-compose
- Documentation odoo : https://hub.docker.com/_/odoo
- Exposer le port 80 du conteneur odoo à l'exterieur
- Faire en sorte que le conteneur odoo et la db soient dans le même réseau bridge nommé odoo_network 
- Vérifier l'acces à l'application odoo

## docker-compose for **odoo and **postgres
installer docker-compose **for linux https://docs.docker.com/compose/install/

```sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose```

```sudo chmod +x /usr/local/bin/docker-compose```
### créer un réseau nommé odoo_network
```sudo docker network create -d bridge odoo_network```

### docker-compose.yml
dans même repertoire que docker-compose.yml
```docker-compose -d up```

### accedrer à l'aplication via le navigateur
```@ip:80```


## créer une image de l'appli visagesanimesjs avec un Dockerfile
(https://github.com/bakidjan/PL2_AI/tree/master/visagesAnimesjs) 

installer docker avec le script : https://get.docker.com/
```curl -fsSL https://get.docker.com -o get-docker.sh```
```sh get-docker.sh```

### Builder l'image
```sudo docker build -t visagesanimesjs .```

### Docker run pour lancer le conteneur à base de l'image
```sudo docker run --name nomimage:version -d -p 8081:80 visagesanimesjs```

### accedrer à l'aplication via le navigateur
```@ip:8081``` 


