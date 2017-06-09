# challenge_selection
Si vous lisez ceci, c'est que vous avez déjà fait connaissance avec le processus de sélection des candidats.
Voici donc venue l'occasion d'aborder celui-ci afin de le rendre plus pratique mais aussi plus ludique.

## Présentation de l'existant
Le processus actuel se découpe essentiellement en trois parties :
* renseigner ses coordonnées,
* répondre à un questionnaire,
* passer des badges sur codecademy.

## Expression du besoin côté candidat
Toutes les étapes de sélection doivent se faire sur la même plateforme.  
Celle-ci propose l'accès standard pour les candidats.

### Inscription
L'inscription est ouverte aux candidats. Pour cela, ils renseignent :
* Nom/prénom  
* Adresse mail  
* Mot de passe (+ confirmation)
* Numéro de téléphone  
* Adresse postale  (+ code postal + ville)
* Sexe
* Date de naissance

(+ CAPTCHA)

Ce processus est suivi de l'envoi d'un mail de confirmation.
Toutes les données liées au statut (demandeur d'emploi ou autres) n'entrent pas dans le cadre du challenge.
Dès sa première connexion, le candidat se voit attribuer un score de 0% et l'accès aux trois volets : profil, questionnaire et badges.

### Badges   
[S'appuyer sur le badge buster de Maxime.](https://github.com/MaximePawlakFr/badge-busters-front)

Attention, ça ne marche pas en l'état parce qu'il manque une API fonctionnelle.
L'objectif ici est d'afficher au moins le nombre de badges récoltés par le candidat. Ce total se rafraîchit à chaque connexion de celui-ci et à chaque consultation de son profil.
**Chaque badge obtenu fait monter le score d'1%.**

### Profil  
Sur cette page, le candidat est amené à renseigner plusieurs champs le concernant :
* Photo
* Expériences professionnelles, diplômes et formations
* Compétences
* Savoir-être/qualités
* Loisirs

**Pour chaque champ renseigné, le score du candidat augmente de 5%.**

### Questionnaire  
Là, le candidat répond à dix questions.
Des exemples de questions sont fournis dans le fichier Excel mis à disposition sur le repository.
**Pour chaque question à laquelle il a répondu, le score du candidat augmente de 5%**  

### Remarques globales  
Le candidat doit pouvoir sauvegarder sa saisie à n'importe quel moment pour reprendre celle-ci plus tard.   
Bonus : la sauvegarde peut-elle être automatisée?
Une fois qu'il a dépassé un certain score, le candidat se voit offrir la possibilité de soumettre sa candidature. Celle-ci est alors envoyée aux formateurs affecté à cette campagne de sélection.
Jusqu'à la date de clôture de la campagne, il peut à nouveau envoyer sa candidature.
Une fois la date de clôture dépassée, il est impossible d'envoyer une nouvelle candidature ou de mettre à jour une candidature existante.   
Attention : le score d'un candidat ne peut pas dépasser 100% mais il n'y a pas de limite max pour les points accumulés via les badges.

## Expression du besoin côté administrateur  
L'administrateur peut affecter des formateurs à une campagne de sélection.
Il peut également visualiser tous les profils des candidats ainsi que les notes qui leur ont été attribuées.  

## Expression du besoin côté formateur  
Le formateur a un profil simple pour se connecter :
* Nom/prénom  
* Adresse mail  
* Mot de passe (+ confirmation)

Le formateur peut consulter les profils envoyés par les candidats correspondant à la campagne à laquelle il a été affecté.
Le formateur peut noter chaque profil selon un barême à définir, en commun avec les autres formateurs de la même campagne.
Les autres formateurs de cette campagne peuvent visualiser les notes attribuées aux candidats.
Un moteur de tri et de recherche permet de n'afficher qu'un certain nombre de critères en fonction de critères à définir (sexe, date de naissance, code postal, score, nombre de badges, etc).

## Consignes  
* Vous n'avez que quelques jours alors soyez organisés.
* Chaque promo bosse en commun sur ce projet alors soyez organisés.
* Astuce : n'hésitez pas à faire un Taïga/Trello.
* Chaque équipe de formateur vous fournira la date de rendu. N'oubliez pas de leur envoyer le résultat à temps avec le repo github et le lien vers la version en ligne.
* Chaque promo doit faire un point projet par mail chaque jour (ce qui a été fait, ce qui reste à faire, quels problèmes ont été rencontrés), à destination de l'ensemble de vos formateurs.
* Faites quelque chose de responsif et de **ludique**. [Le game design, ce n'est pas si difficile.](https://github.com/SimplonSt-Gaudens/programme-web-dev/wiki/Semaine-10-:-game-design)
* Débrouillez-vous.
