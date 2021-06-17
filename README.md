The objective of the project is to set up a micro-service web application on a cluster infrastructure

# Installation de l'infrastructure

## Déploiement de Docker Swarm avec Ansible

### Les prérequis

1) Installation d'Ansible via le gestionnaire de paquets.


### Le déploiement

1) En dev :

```console
user@client:~$ ansible-playbook -i dev/inventory  -u user infrastructure.yml --ask-become-pass --vault-id .vaultfile
```

2) En prod :

```console
user@client:~$ ansible-playbook -i prod/inventory  -u user infrastructure.yml --ask-become-pass --vault-id .vaultfile
```
