
# TEAM HTTP 413 / SUJET IST NDI 2022 : Application No mISTery

## Notre choix technique

Nous avons choisi de partir sur une forme de site web hébergeant une multitude de mini jeux tournés autour de la sensibilisation sur le maximum d'IST possible, comportant à chaque fois de petits messages de prévention que l'utilisateur gagne ou perde.

Les principes sont simples, détourner des jeux classiques que tout le monde connais pour faire apprendre à notre publique sans qu'il ne s'en rende compte.
Notre publique cible est clair, les adolescent à partir de 13 ans, soit la classe de 4eme, ou les cours d'éducation sexuelle commencent.

Pour cela, nous avons conçu 4 jeux que vous retrouverez sur notre pateforme :

- **Dépisteur** :

Jeu ou vous devez jouer à un démineur à l'aide de la souris, en découvrant le plateau grace au clic gauche et en posant des marqueurs ( qui ne sont autre que des préservatifs ) sur les cases piégées par des ISTs. Si vous cliquez malheureusement sur une des IST, votre barre de vie descend. Si vous cliquez sur trop d'ISTs, vous perdez la partie et un message de prévention aléatoire apparait. Sinon, vous gagnez la partie et vous avez accès à un leaderboard contenant le message de prévention de victoire. Un lien externe de documentation supplémentaire est également présent.

- **IST Clicker**

C'est un simple jeu de clicker demandant à l'utilisateur d'éliminer des IST en cliquant de nombreuses fois dessus, dans un temps imparti. Plus l'utilisateur en élimine, plus il marque de points. Une fois la partie terminée, un petit message de prévention s'affiche contenant des statistiques sur les IST en France ou dans le monde. Un lien externe de documentation supplémentaire est également présent.

- **MemeCapote**

C'est un jeu de mémory comme nous en avons tous fait enfant, sauf que cette fois il faut etre attentif a de petits détails, auquel une personne confrontée dans le vie réelle à cette situation devra etre attentive. En effet, de nombreux détails sont présents sur les préservatifs, tels que la date de péremption par exemple, et l'utilisateur doit essayer de s'y retrouver pour trouver les préservatifs ne présentant pas de danger à l'usage. Une fois sont choix fait, un message apparait en fonction de s'il à fait le bon choix ou non, et il à accès également à un leaderboard. Un lien externe de documentation supplémentaire est également présent.

- **Morpion**

C'est un jeu de morpion, mais avec des morpions ! Jouable par deux utilisateurs l'un contre l'autre, des morpions et des rasoirs s'affrontent... En fonction de quel utilisateur gagne la partie, un message de prévention différent s'affiche, et le leaderboard est accessible. Un lien externe de documentation supplémentaire est également présent.


## Notre équipe

Nous étions une équipe de 18 étudiants, répartis selon les fonctions suivantes :

- Un chef de projet
- Des leads fronts et back ainsi qu'un manager gérant les teams
- Des teams front et back ainsi qu'une team agile qui navigue entre les deux
- Un responsable cybersécurité
- Une team de designers responsable de toute la partie UX de l'application et de sa charte graphique

L'ensemble des 18 personnes à pu contribuer au projet et nous sommes extrèmement fiers d'avoir pu coordonner autant d'étudiants sur un projet commun de cette ampleur.


## Fonctionnalitées implémentées

Les fonctionnaliées implémentées sont les suivantes :

- Une page d'administration permettant de modérer le leaderboard
- Les minis jeux de prévention et la gamification

De manière plus large nous avons implémenté la totalité du sujet de la nuit.


## Notre rendu

Notre site de rendu est disponible sur la page suivante :

https://www.team2large.fr

La page d'administration est en bas à droite de la page principale ou ici :

https://www.team2large.fr/admin/login

avec aucun login, comme password :

"945239b7e4089692160a3e58225f04830c58dd9853bfb2d0279152881ba0c778"
( ne tapez pas le responsable cyber la page admin n'a aucune importance en terme de cyber )

Cela dit, nous avons implémenté le défi local qui consiste à avoir l'authentification la plus longue et ridiculement difficile possible, nous vous souhaitons donc beaucoup de plaisir pour vous connecter !

La liste des **routes de l'API** est la suivante :
https://api.team2large.fr
- GET : /games - liste des jeux
- POST : /games/:slug/scores - prend en paramètre le score et l'username à enregistrer sur un jeu donné en paramètre d'url
- GET : /games/:slug/scores - liste les scores du jeux identifié par {slug}
- DELETE : /admin/scores/:id - delete le score correspondant à l'id donné en paramètre
- GET : /admin/scores - liste tous les scores, tout jeux confondu
- POST : /admin/login - prend en paramètre le password hash et le compare à celui dans le .env pour la connexion administrateur
- GET : /tools/refresh - initialise la base de données, avec les jeux prévu 

## Les défis relevés

Nous avons décidé de relever 4 défis au total :
- Le défi de la nuit de l'info en lui même que nous avons terminé
https://www.nuitdelinfo.com/inscription/defis/174

- Le défi local qui consiste à avoir l'authentification la plus ridiculement complexe possible, par KBDev :
https://next.kbdev.io/ndi22

- Le défi cybersécurité de PROXYM : 
https://www.nuitdelinfo.com/inscription/defis/364
https://drive.google.com/file/d/1a30xXN9KEM2iA02iJKek_7pVH_G2Od-u/view?usp=share_link

- Le défi easter egg de l'ASI RENNES :
https://www.nuitdelinfo.com/inscription/defis/302

Celui-ci peut etre trigger en glissant le préservatif de l'écran d'accueil présente à gauche du nom du site sur le virus présent à droite du nom du site. Enjoy !


