### **# fichiers-de-configuration-ci-cd**  

## **Commandes utilisées dans notre vidéo**  

```bash
$ wget https://Bucket-name.s3.Region-identifier.amazonaws.com/latest/install
```

##### Ensuite, nous devons modifier les permissions du fichier d’installation que nous avons téléchargé avec la commande précédente :  

```bash
$ chmod +x ./install
```

##### Enfin, pour installer l’agent CodeDeploy, exécutez cette commande :  

```bash
$ sudo ./install auto > /tmp/logfile
```

###### Ici, nous enregistrons la sortie de l’installation dans le fichier `/tmp/logfile`. Pour vérifier si l’agent CodeDeploy est en cours d’exécution, entrez cette commande :  

```bash
$ sudo service codedeploy-agent status
```

###### S'il n'est pas en cours d'exécution, utilisez cette commande pour démarrer le service CodeDeploy-agent :  

```bash
$ sudo service codedeploy-agent start
```

