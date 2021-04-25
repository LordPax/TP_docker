# Docker - TP8 : Autonomie avec Docker-Compose
> **Objectifs du TP** :
>- Manipulation de l'outil docker-compose
>

## 1 - Docker-compose

Créez un fichier `docker-compose.yaml`avec 4 services nginx:
`nginx-toto` qui expose sur le port 3000 un fichier HTML comportant "Hello Toto" récupéré de votre poste localhost.
`nginx-tata` qui expose sur le port 3001 un fichier HTML comportant "Hello Tata" récupéré de votre poste localhost.
`nginx-titi` qui expose sur le port 3002 un fichier HTML comportant "Hello Titi" récupéré de votre poste localhost.
`nginx-tutu` qui expose sur le port 3003 un fichier HTML comportant "Hello Tutu" récupéré de votre poste localhost.

Pour exécuter votre code vous pouvez lancer la commande suivante : `docker-compose up -d`
- `up` : Créer la stack
- `-d` : Lancer en tâche de fond
- `--build` (Situationnel): Permet de rebuilder les images (Dockerfile)

Vérifiez que vous avez bien le comportement suivant :
```bash
$ curl localhost:3000
> Hello Toto`

$ curl localhost:3001
> Hello Tata`

$ curl localhost:3002
> Hello Titi`

$ curl localhost:3003
> Hello Tutu`
```
