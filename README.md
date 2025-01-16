# Créer et lire des enregistrements en BDD

Dans cet atelier, tu vas aider Père Blaise à écrire l'histoire des chevaliers de la table ronde !  
Pour cela, tu vas récupérer et créer des informations en base de données avec PHP et PDO !
{: .alert-info }


## Mise en place

Connecte-toi à la base de données nommée `kaamelott` que tu as créée lors du précédent atelier (ou recrée-là si besoin).   

En utilisant le client MySQL CLI (dans ton terminal), crée une table `story` contenant les champs suivants avec les types que tu juges appropriés.
- `id` integer, clé primaire autoincrémentée
- `title` chaîne, max 255 caractères
- `content` texte
- `author` chaîne, max 100 caractères

## Ajouter une histoire
Créer un fichier *create.php* contenant un formulaire HTML permettant de renseigner chaque information d'une histoire (titre, contenu, auteur).  

À la soumission du formulaire dans *create.php*, insérer la saisie de l'utilisateur en base de données grâce à PDO.
Appuie-toi sur l'utilisation de PDO que tu viens de voir, ainsi que ce que tu as déjà fait auparavent :  
- insertion en base de données à l'aide de SQL et manipulation de formulaires HTML.
- sécuriser les entrées à l'aide des requêtes préparées de PDO

## Lire une histoire
Créer une page *index.php*, affichant la liste des histroires contenus en base de données. 
Encore une fois, appuie-toi sur l'utilisation de PDO que tu viens de voir, mais également sur ce que tu as déjà fait auparavant&nbsp;:
- récupération en base de données et parcours de tableaux en PHP 
- sécuriser l'affichage contre les failles XSS
