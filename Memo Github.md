## CONFIGURATION DES OUTILS
### Configurer les informations de l'utilisateur pour tous les dépôts locaux
```
$ git config --global user.name "[nom]"
```
Définit le nom que vous voulez associer à toutes vos opérations de commit
```
$ git config --global user.email "[adresse email]"
```
Définit l'email que vous voulez associer à toutes vos opérations de commit
```
$ git config --global color.ui auto
```
Active la colorisation de la sortie en ligne de commande

## CRÉER DES DÉPÔTS
### Démarrer un nouveau dépôt ou en obtenir un depuis une URL existante
```
$ git init [nom-du-projet]
```
Crée un dépôt local à partir du nom spécifié
```
$ git clone [url]
```
Télécharge un projet et tout son historique de versions

## EFFECTUER DES CHANGEMENTS
### Consulter les modifications et effectuer une opération de commit
```
$ git status
```
Liste tous les nouveaux fichiers et les fichiers modifiés à commiter
```
$ git add [fichier]
```
Ajoute un instantané du fichier, en préparation pour le suivi de version
```
$ git reset [fichier]
```
Enleve le fichier de l'index, mais conserve son contenu
```
$ git diff
```
Montre les modifications de fichier qui ne sont pas encore indexées
```
$ git diff --staged
```
Montre les différences de fichier entre la version indexée et la dernière version
```
$ git commit -m "[message descriptif]"
```
Enregistre des instantanés de fichiers de façon permanente dans l'historique des versions

## CHANGEMENTS AU NIVEAU DES NOMS DE FICHIERS
### Déplacer et supprimer des fichiers sous suivi de version
```
$ git rm --cached [fichier]
```
Supprime le fichier du système de suivi de version mais le préserve localement
```
$ git rm [fichier]
```
Supprime le fichier du répertoire de travail et met à jour l'index
```
$ git mv [fichier-nom] [fichier-nouveau-nom]
```
Renomme le fichier et prépare le changement pour un commit
