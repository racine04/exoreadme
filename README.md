***************PROCESSUS DE CREATION D'UN PROJET DJANGO***************


*PREREQUIS*
-python
-un editeur de code

I. *ENVIRONNEMENT VIRTUEL*
Pour l'utilisation du framework Django il est essentiel de se trouver dans un environnement virtuel


1. *Création de l'environnement virtuel*
Pour la création d'un environnement virtuel nous devons:
-Ouvrir le dossier dans lequel nous voulons utiliser le framework django avec un editeur de code de préférence VS Code

-Ouvrir un nouveau terminal

-Entrez la commande : *python -m venv nom_envi* (nom_envi doit etre remplacer par le nom de votre environnement)

2. *Activation de l'environnemnt virtuel*
Apres avoir creer l'environnement virtuel nous devons l'activer pour se faire nous devons:

-Entrez la commande *nom_envi/Scripts/activate*

II. *Framework Django*

1. *Installer Django*
Une fois passer cette etape il nous faut maintenant installer Django le framework que nous allons utiliser pour ce faire nous utilisons la commande:

-*pip install django*

2. *Creer un projet Django*
Une fois django installe nous pouvons maintenant creer notre projet django avec la commande
- *django-admin startproject nom_projet* (remplacer nom_projet par le nom de votre projet)

III. *Apllication Django*

1. *Creation de l'application*
Pour creer l'application nous devons tout d'abord entrer dans le dossier du projet avec la commande:

-*cd nom_projet*

- et ensuite creer l'application avec la commande :*django-admin startapp nom_app* (remplacer nom_app par le nom de l'application)

IV. *Creation des vues de l'application*

1. *Integration du l'application au projet*
Pour integrer l'application au projet nous devons:
- nous rendre dans le setting du dossier portant le meme nom que nostre projet dans la partie nommee *INSTALLED_APPS* et ajouter le nom de l'application a la suite des applications deja installe

2. *Creation du dossier templates*
-Une fois l'application integre nous devons creer un dossier nomme *templates* dans le dossier de mon application *nom_app*

-Apres avoir cree le dossier nous pourrons ajouter tous nos fichiers *HTML* dans ce dossier *templates*

3. *Creation des vues*
Pour la creation des vues nous devons nous rendre dans le fichier *views* de l'application qui comporte deja les modules a importer et creer des fonctions qui reverront nos fichiers *HTML* contenu dans notre dossier *templates* 
Prenons l'exemple d'un fichier *index.html* contenu dans notre dossier *templates* et nous voulons renvoyer cette fonction la fonction qui permettra de le faire peut etre:

*def* index(*request*):
 return render(*request*, index.html)

4. *Creation des URL*
Nous devons maintenant etablir des liens qui nosu permettrons d'acceder a nos vue et pour cela nous creons un fichier *URLS* dans notre application et 




