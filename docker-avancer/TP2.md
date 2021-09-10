
# Docker - TP2 : Gestion des networks avec Docker-Compose
> **Objectifs du TP** :
>- Manipulation des networks avec docker-compose
>

## 2 - Gestion des Networks 

> Ce TP fait suite au TP1 (il faut donc avoir terminé le TP1 avant de réaliser celui-ci)

Vous devriez donc avoir un fichier `docker-compose.yaml` comportant 4 services avec l'image nginx.
Modifiez votre fichier `docker-compose.yaml`de façon à ce que : 
- `nginx-toto` puisse communiquer avec `nginx-titi` mais pas `nginx-tata` ni `nginx-tutu`
- `nginx-tutu` puisse communiquer avec `nginx-titi` mais pas `nginx-toto` ni `nginx-tata`
- `nginx-titi` puisse communiquer avec `nginx-tata`,`nginx-toto`, `nginx-tutu`

Par le moyen de la commande `curl` exécutez les commandes permettant de prouver l'isolation de vos services après la mise en place des networks demandés. 
