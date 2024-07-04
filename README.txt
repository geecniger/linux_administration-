Processus Principal :

Vérifie si une URL cible est fournie, sinon affiche un message d'erreur et termine.
Définit le domaine à partir de l'argument.
Récupère la référence de la branche HEAD à partir du dossier .git de l'URL fournie.
Récupère le dernier hash du commit de cette référence.
Initialise un nouveau dépôt Git local.
Change de répertoire pour le dossier .git/objects/.
Appelle parseCommit sur le dernier hash du commit.
Retourne au répertoire racine.
Écrit le hash du dernier commit dans .git/refs/heads/master.
Réinitialise le dépôt pour correspondre au dernier commit téléchargé.
Utilisation du Script
Pour utiliser ce script, exécutez-le avec une URL d'un site ayant un dossier .git accessible :

bash
Copier le code
./scrabble.sh http://example.com/
Conclusion
Ce script illustre comment l'accès non sécurisé à un dossier .git peut compromettre l'intégrité 
et la sécurité de votre code source. En production, il est crucial de s'assurer que le dossier .git n'est 
pas accessible publiquement pour éviter de telles exploitations. Utilisez ce script dans un environnement 
contrôlé et sécurisé pour des démonstrations éducatives seuleme
