`	`**TP2 UNIX – LINUX**	

**Droits Utilisateurs**
# **Droits d’accès aux fichiers**
- **Vous disposez de deux terminaux supplémentaires accessibles par Ctrl-Alt-F5 et Ctrl-Alt-F6**
- **Le retour à l’interface graphique se fait par Ctrl-Alt-F7**
- Il est possible d'ouvrir une session sous l'utilisateur tux grâce à la commande : 
  sudo -i -u tux	(terminer la session par Ctrl-D)
- Il est possible d'ouvrir une session sous le super-utilisateur root grâce à : 
  sudo -i	(terminer la session par Ctrl-D)

  1  ## ***Comptes utilisateurs et groupes***
1. Créer un nouvel utilisateur tux. Créer le dossier personnel de tux en utilisant l’option appropriée (indication : utiliser la commande useradd)
   *NB: tant qu’on n’a pas attribué un mot de passe au nouvel utilisateur , il ne pourra pas ouvrir de session*
1. Affecter à tux le mot de passe mdptux (indication : utiliser la commande passwd)
1. Afficher votre nom de connexion et votre UID (Indication : utiliser la commande id)
1. Procéder de même pour les comptes tux et root.
1. Afficher les groupes auxquels vous appartenez (Indication : utiliser la commande groups).
1. Procéder de même pour les comptes tux et root.

1  ## ***Droits par défaut***
1. Dans votre répertoire personnel, créer un répertoire portant le nom tp2.
1. Afficher les droits d'accès sur votre répertoire tp2 (Indication : utiliser la commande ls avec l'option qui convient).
1. Afficher le masque définissant les droits par défaut lors de la création de fichiers. Que signifie la valeur affichée (Indication : utiliser la commande umask) ?
1. Aller dans votre répertoire tp2 puis créer un fichier vide fic1 et un répertoire rep1.
1. Les droits du fichier fic1 et du répertoire rep1 correspondent-ils à la valeur du masque affiché précédemment ?
1. Modifier votre masque définissant les droits par défaut à la valeur 27. Que cela signifie-t ‘il ?
1. Créer un fichier vide fic2 et un répertoire rep2.
1. Vérifier que les droits du fichier fic2 et du répertoire rep2 correspondent à la nouvelle valeur du masque. Les droits du fichier fic1 et du répertoire rep1 ont- ils changés ?

1  ## ***Droits des répertoires***
1. Donner les droits r, w, et x aux autres utilisateurs sur le répertoire rep1 en utilisant la notation symbolique.
1. Donner les mêmes droits que le répertoire rep1 à rep2 en utilisant la notation octale.
1. Créer le répertoire /tmp/ubuntu. Lui donner aussi les mêmes droits qu'aux répertoires rep1 et rep2 précédents.
1. Créer le fichier secret dans le répertoire /tmp/ubuntu.
1. Se connecter sur une seconde console virtuelle texte (<a name="_hlk156312362"></a>touches Ctr-Alt-F5) en tant qu'utilisateur tux.
1. En tant qu'utilisateur tux, pouvez-vous lire le fichier secret de linux ?
1. Retourner sous l'identité de l'utilisateur linux sur la première console (Ctr-Alt F7) virtuelle texte
1. Modifier les droits du fichier secret de manière à ne laisser le droit de lecture qu'à l'utilisateur **tux**. Pour cela, changer le propriétaire du fichier (commande chown)
1. Retourner sous l'identité de l'utilisateur tux sur la deuxième console (Ctr-Alt F5) virtuelle texte
1. Pouvez-vous supprimer le fichier secret? Pourquoi ?

   1  ## ***Droits et liens***
1. Retourner sous l'identité de l'utilisateur ubuntu sur la première console (Ctr-Alt F7) virtuelle texte et retourner dans le répertoire /home/etudiant/tp2.
1. Positionner votre masque à la valeur 002.
1. Créer le répertoire docperso et lui affecter les droits 700.
1. Aller dans le répertoire docperso et créer les fichiers fica, ficb, ficc et ficd. Puis lister de façon détaillée le contenu du répertoire.
1. Créer le lien dur (« hard link ») /tmp/lienfica vers le fichier fica et le lien symbolique (« soft link ») /tmp/lienficb vers le fichier ficb (Important : Veillez à créer un lien symbolique valide en utilisant des chemins d'accès absolus).
1. Retourner sous l'identité de l'utilisateur tux sur la seconde console virtuelle et essayer de lister le contenu du répertoire /home/etudiant/tp2/docperso. Est-ce possible et pourquoi ?
1. Afficher le contenu du fichier /tmp/lienfica. Est-ce possible et pourquoi ?
1. Afficher le contenu du fichier /tmp/lienficb. Est-ce possible et pourquoi ?

`	`***3iL***	Page 3/3
