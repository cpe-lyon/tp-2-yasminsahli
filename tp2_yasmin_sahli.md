Yasmin SAHLI ICS 

# TP2 BASH

## Exercice 1. Variables d’environnement

1. Les commandes tapées par l'utilisateur se trouvent dans les dossiers : 
```

/usr/local/sbin
/usr/local/bin
/usr/sbin
/usr/bin
/sbin
/bin
/user/games
/usr/local/games
/snap/bin
```

2. La variable d'environnement qui permet à la commande cd de nous ramener dans notre répertoire personnel est la variable $HOME. (printenv HOME)


3. La variable LANG contient la langue utilisée par le système.

La variale PWD contient le chemin du répertoire courant. (répertoire courant : répertoire qui fait l'objet de l'opération en cours à un moment donné et que le système choisit par défaut)

La variable OLDPWD contient le chemin de l'ancien répertoire courant. 

La variable SHELL contient l'interpréteur de commande utilisateur défini dans "/etc/passwd".


4. Pour créer ma variable locale j'ai fais : MY_VAR="ma variable pour la question 4"

Et pour vérifier que la variable existe j'ai fais echo $MY_VAR


5. La commande bash lance un nouvel interpréteur de commande. Donc quand on fait echo $MY_VAR rien ne s'affiche car on a créer la variable comme une variable locale.



6. Pour transformer la variable en variable d'environnement on fait : export MY_VAR="ma variable pour la question 4"

Et désormais lorsqu'on retape la commande bash et que l'on fait echo $MY_VAR on a bien récupéré le contenu de cette variable, et cella confirme bien le fait qu'elle n'est plus une variable locale mais une variable d'environnement.


7. Pour créer la variable d'environnement nom j'ai fais : export NOM="Yasmin SAHLI"

Et pour que l'affectation est correcte j'ai fais printenv NOM. Le contenu de la variable s'est affiché donc l'affectation est correcte. 


8. Pour afficher un texte en utilisant la variable NOM on crée un script bash.

On a tapé : 
```

#!/bin/bash

echo 'Bonjour à vous,' $NOM '!'
```

Et on a le message qui s'affiche avec mon Prénom et mon nom.

J'ai fais : 
```
nano message.sh 
```
Puis j'ai retapé cette commande echo 'Bonjour à vous,' $NOM '!' dans le fichier message.sh

Et maintenant pour que mon message s'affiche il suffit juste de taper :
```
./message.sh
```

9. La commande "unset" supprime la variable d'environnement alors que donner une valeur vide à une variable ne la supprime pas cette dite variale.


10. J'ai fais :
```
echo '$HOME' = "$HOME"
```

et j'ai obtenue $HOME = /home/User


## Exercice 2. Contrôle de mot de passe

Pour créer le chemin permanent au PATH vers script j'ai fais : 
```
PATH=$PATH:~/script
```
Et le code pour la saisie de mots de passe est le suivant : 

<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022135982126014544/exo2bis.png">
<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022135543116603432/exo_2_.png">

## Exercice 3. Expressions rationnelles

<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022136282488516639/exo3.png">

<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022136282945683506/exo3_bis.png">

## Exercice 4. Contrôle d’utilisateur

Écrivez un script qui vérifie l’existence d’un utilisateur dont le nom est donné en paramètre du script. Si le
script est appelé sans nom d’utilisateur, il affiche le message : ”Utilisation : nom_du_script nom_utilisateur”,
où nom_du_script est le nom de votre script récupéré automatiquement (si vous changez le nom de votre
script, le message doit changer automatiquement)

<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022136968227860480/exo4.png">

<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022136968768913478/exo4bis.png">

## Exercice 5. Factorielle

Écrivez un programme qui calcule la factorielle d’un entier naturel passé en paramètre (on supposera que
l’utilisateur saisit toujours un entier naturel).

<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022137193352929380/exo5.png">
<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022137193952727093/exo5bis.png">

## Exercice 6. Le juste prix

Écrivez un script qui génère un nombre aléatoire entre 1 et 1000 et demande à l’utilisateur de le deviner.
Le programme écrira ”C’est plus !”, ”C’est moins !” ou ”Gagné !” selon les cas (vous utiliserez $RANDOM)

<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022137548069412884/exo6.png">
<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022137548476272660/exo6bis.png">

## Exercice 7. Statistiques

<img src ="https://cdn.discordapp.com/attachments/752464625576050780/1022137718731456513/exo7.png">


