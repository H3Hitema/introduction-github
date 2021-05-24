# Introduction à GitHub

Ce README résume le module de cours sur GitHub disponible sur le LMS de H3 Hitema. 

## Qu'est ce que GitHub 

GitHub est avant tout une plateforme d'hébergement de code. On peut le voir comme le "google drive" (outils de stockage en ligne de google) pour le code. Il permet aussi la gestion de version et la collaboration. 


## Créer un nouveau dépot (repository)

Un repository ou un dépot (dossier qui contient du code) est généralement utilisé pour organiser un seul projet. Les repository peuvent contenir des dossiers et des fichiers, des images, des vidéos, des feuilles de calcul et des ensembles de données, globalement tout ce dont votre projet a besoin pour fonctionner. 

Créez un nouveau dossier, ouvrez le et exécutez la commande
```
git init
```

## Cloner un dépôt


Créez une copie de votre dépôt local en exécutant la commande
```
git clone /path/to/repository
```

## Ajouter & valider du code dans un dépot
Pour un fichier utilisez 
```
git add <filename>
```
Pour ajouter tous les fichiers 
```
git add *
```

### Pour valider vos changements, utilisez
```
git commit -m "Message de validation"
```

## Envoyer des changements sur une branche (master par défaut)
Pour envoyer vos changement à votre dépôt distant, exécutez la commande
```
git push origin master
```

## Les branches 
Les branches sont utilisées pour développer des fonctionnalités isolées des autres. La branche master est la branche par défaut quand vous créez un dépôt. 

### Créer une branche sur votre dépot 
Pour créer une nouvelle branche nommée "feature_x" et passer dessus pour l'utiliser
```
git checkout -b feature_x
```

### Retourner sur votre branche principale
```
git checkout master
```

### supprimer la branche
```
git branch -d feature_x
```
🚧 **Attention une branche n'est pas disponible pour les autres tant que vous ne l'aurez pas envoyée vers votre dépôt distant** 🚧

### La petite astuce pour la fin 
Pour ceux qui n'arrivent pas à pull parce qu'ils ont fait des modif dans le repo, lancer la commande : 
```
git stash
git pull
git stash pop
```

