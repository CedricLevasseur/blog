Title: Compte rendu de Paris Web 2015
Date: 2015-10-04 18:30
Tags: paris-web
Category: paris-web
Author: Cédric Levasseur
Summary: Avec des licornes dedans !


Ceci est un prise de note des conférences, avec mon avis sur le déroulement.
Vous pouvez sauter directement à la [conclusion](#conclusion) 


Jour 1
======


Internet et libertés : pour un engagement des acteurs du numérique
------------------------------------------------------------------

_Par Adrienne Charmet_

Première entrée de la politique pour Parisweb, puisqu'il s'agit de présenter la Quadrature du net.

_Mon avis :_ J'avoue avoir été déçu et sur la réserve. Toutefois, je partage l'opinion de la Quadrature du net. Est-ce l'exhaustivité d'Adrienne qui m'a ennuyé ?
Est-ce le manque de slides ? Est-ce l'engagement politique qui me fait peur ? Sans doute un peu, Quoiqu'il en soit je ne peux pas laisser nos libertés se faire bafouer sans réagir. Je devrais un jour me positionner.


Service worker
--------------

_Par Eric Daspet_

C'est l'histoire d'un site web qui gère le offline, au lieu de télécharger une application native sur mon téléphone. Pour cela il utilise service worker. De plus on peut même faire du offline-first ou du analytics-offline. 
Idem on peut lire le zip d'un epub.
Autre avantage, quand service worker n'est pas implémenté dans le navigateur (exemple de Safari), on reste sur le site web normal.
Geofencing : Réveiller une application web quand on se trouve à un endroit prédéfini.
Les Service workers sont aussi important que l'arrivée d'Ajax.

_Mon avis :_ Présentation claire. Aurait mérité plus de temps et plus d'exemples de code.


Formulaire Web
--------------

_par Stépĥane Borzmeyer_

Acceptation générale et acceptation universelle.
"Vous êtes nul et ce que vous faites est très mal" en parlant de la validation des formulaires.
exemple : une adresse email avec un TLD récent.
Une regexp pour tester le nom de domaine 

_Mon avis :_ Stéphane est très provocateur et très drôle. Je ne le connaissais que par twitter.

_Une idée à implementer_ : Un plugin pour forcer ces regexp idiotes à retourner ``true``


CSS grid Layout
---------------

_Par Rachel Audrew_ 

Utiliser CSS grid layout, cela ressemble à une mise en page en tableau, mais c'est dans la CSS.
On peut nommer les colonnes. La syntaxe est un peu étrange pour définir des colonnes, des goutières.. avec des slashes.
Il y a aussi un nouveau mot clé ``repeat``. ``dense`` Un nouvelle unité ``fr`` pour fraction.
On peut faire très facilement du prototypage ou refaire des redispositions plus facilement. A condition de maîtriser !
Cette innovation arrivée dans IE10 et la spécification n'est pas terminée. 
gouttière vs marge ? Gouttière est une cellule vide plus courte pour séparer deux colonnes.
On peut faire des grilles imbriqués, dans la première version, il y avait un mot clé subgrid, mais pas encore implementée.

_Mon avis :_ Une présentation assez visuelle, qui montre cette révolution de CSS grid Layout.
Très intéressant beaucoup d'infos. Présentation bien rodée, la présention manque peut-être un peu de fantaisie. 


Hey, tu peux reprendre mon projet ?
-----------------------------------

_Par Sylvain Zysman_

_Mon avis :_ Conférence amusante, avec quelques généralités. Je n'en n'ai pas retenu grand chose (Désolé). 



Le RUN (ou TMA)
---------------

_Par Leila Touati_

- Réactivité
- Maintenance préventive (Note : AHAHAH ça existe ça ? ). Ne pas oublier que certaines personnes sont mal intentionnée. Lire les logs :)
- Maintenance adaptative : monte de version de navigateur et d'OS mobile. Il faut donc impliquer le client : Audit, devis...
- Exploitation : 

_Mon avis :_ Des extraits de film viennent aggrémenter cette conférence, plaisante. Je comprends un peu plus ce qu'est que le TMA pour des grosses
applications. Et pourtant j'ai déjà fait de la TMA. Un peu trop orienté sur des ventes de "prestations" et pas assez de technique à mon goût.
Cela dit si je me lance un jour en indépendant, c'est intéressant de savoir ce que je vais vendre, si je vends de la TMA.


Confession d'un Serial Killer
-----------------------------

_Par Virginie Clapet_

Virginie imagine, un sur-moi, ou un tier, sérial killer qui sabotte nos idées.
Vous ne vous faites pas confiance, donc vous faites confiance aux autres. Et les autres vous font confiance. Donc vous ne vous voulez pas les trahir.Bref, vous êtes obligé de vous faire confiance. 
"Fait-le et tu aides quelqu'un en le faisant "

les humains serial-killer : Les boucliers humains, les erreurs de castings, les gate-keepers experts.
les process serial-killer : absence de process ou de but/ Sauter d'un projet à un autre / Absence de diversité (c'est pas naturel)
Mode opératoire pour mettre en échecs ces sérials killers : 
- Couper en petit morceaux : Ne faites pas des gros projets. Minimum Viable Product.
- prendre de la distance dans l'espace-temps. Rapprocher la dateline, 
- DIY c'est has-been. Vive le DIWO : Do It With Other. Echanger !
- Parler avec des inconnus. Ces inconnus vont vous poser des questions. 
- Arrêter de demander la permission. Faites. Si ça foire, demandez pardon. 
- Ne pas pensez que l'on est FutureProof
- Choisissez votre combat : 
- Règle #1 : Ne vous tuez pas.
- Règle #2 : Ne tuez personne
- Règle #bonus : Changez une vie
Les gens qui jugent et qui critiquent sont ceux qui n'ont pas confiance ... en eux

_Mon avis :_ Conf très drôle et plaisante... et très riche. La meilleure conf de la journée à mon avis.
Je pense que je ferais un prochain article de blog là dessus.
Je rapproche aussi ce que m'a dit [Bastien](http://jolicode.com/) également : Personne ne pourra jamais te reprocher d'avoir fait ton maximum (Je faisais allusion à mon perfectionnisme, ma crainte d'être jugé)


De "grands pouvoirs" impliquent de grandes "responsabilités"
-------------------------------------------------------------

_Par Etienne Samson_

_Mon avis :_ Hum... Je n'ai pas retenu grand chose... Décidément, Je n'aime pas les confs sans slides


Etes-vous au top ?
-------------------

Les graphistes ne s'entrainent pas...contrairement aux sportifs, aux militaires, aux musiciens qui font leurs gammes...
Un side-project n'est pas non plus un entrainement, car un entrainement c'est une répétition et sur un petit process.
L'idée c'est d'acquérir un processus.
Les natures de l'entrainement : Physique, Mental... c'est complexe.
Entrainement physique : 
- La mémoire musculaire. L'hypothèse des 10000 heures. Adopter de nouvelles pratiques : écrire dans la main gauche, croiser les mains différements.
- Les routines : 
- La cognition incarnée : notre façon de penser est influencée à la manière dont notre corps est en action. On mémorise mieux un nouveau mot étranger en faisant un geste.  
mémoire visuelle : 
Exploration créative : pensée latéral. Bliz idéation.
Compétences relationnelles : La Résolution des problèmes. Montrer son travail. Apprendre du comportement humain. communication efficace. conscience de soi.

_Mon Avis :_ Ce n'est pas la conf que j'attendais; Ici c'est plus augmenter son savoir faire non technique alors que j'aurais aimer : augmenter son savoir faire technique. Passé mon sentiment de surprise, il y avait plein d'idées interessantes à expliquer, mais le format de la conf était trop court. Aurait mérité plus de temps, ou alors réduire son champ d'action.
La conf sur la veille technique que j'attendais est demain, par Thibault Jouannic.


Panorama des Solution hybride mobile
------------------------------------

_Par Mickael Dumand_

2009 Phonegap = prémisse de l'hybride
2011 Adobe rachète Nitobi
2012 Facebook abandonne html5 pour refaire du natif : Contre-pied ! Depuis, LinkedIn aussi 
2012 : Il n'existe aucun SDK HTML5 pour mobile.
2015 : Il existe deux solutions
1) Solution uniquement javascript : ReactNative et NativeScript
ReactNative
Une couche de javascript lancé sur ios javascript-core ou une partie chrome sur android
Au lien d'utiliser du Html on utilise des balises définies par le framework.
Inconvénient : Framework jeune, 
Avantage : pas de compilation, un refresh siffit à voir le changement
NativeScript : idem

2) Solution de développeur web "natif" : js + css +html5
Phonegap et Cordoba
aussi famo.us : un moteur de rendu, plutôt pour l'évntiementiel 
Onsen UI, un équivalent du bootstrap pour mobile, mais communauté moins forte
TouchstoneJs : Un peu tropjeune.
Ionic : SDK, ommercial, solution mature.
Faut connaitre Apache Cordova, gulp comme task runner, AngularJs, Saas... 
Ionic commence à prendre en compte les spécificités des plateformes Ios / Android
Avantage Ionic est facile à prendre en compte
Hybride c'est l'avenir.
Ionic se base sur une webview.
Crosswalk pour Android a été intégré dans Ionic

Et si l'on veut accéder aux api natives ? C'est possible dans Cordoba.
IOnic a fait ngCordova.

Bref le développement mobile, il faut avoir plein de compétences, différentes.
Et le sujet bouge beaucoup. C'est vraiment pas simple.
Write-once run-anywhere, cela n'est pas encore vrai.
Learn Once, write anywhere, ou aussi Write Once, Adapt for anywhere
Les solutions natives restent plus performantes que ces solutions. Tout dépends aussi de l'application.  
Les solutions Hybrides sont vraiment pour des petits projets.
Anoter aussi que Ionic a prévu de sortir sur Angular 2. Mais Angular 2 met du temps à sortir malgré l'annonce de sa sortie.
A noter Apache Cordova c'est le code source libéré de Phonegap.


Pourquoi on fait des applications pour mobiles, c'est parce que l'on veut utiliser le hardware. Donc le hybride ne peut pas tout.
A noter : il existe aussi des solutions cross-platform ou l'on recompile des applications natives. Solution souvent payantes.

_Mon avis :_ Un conf intéressante, peut-être un peu rapide. Manque de démo. Le sujet est très compliqué et méritait bien cette conf pour y voir plus clair. Le problème c'est que ca évolue très vite. Et que je ne me souviendrais plus de rien si faire du mobile me tentais.


JOUR 2
=======


Quoi de neuf sous le ciel de la sécurité du web et des internets.
------------------------------------------------------------------

_Par Virginie Galindo_ 

La sécurité c'est de la technique, il faut que l'on soit plus didactique
Le monde de la finance est celui qui est le plus demandeur de sécurité.

Intéressant, un certificat gratuit : letsencrypt.org ou CSR qui lui n'était pas accepté.

_Mon avis :_ Quelques arguments me choquent : La sécurité n'a pas à être la même pour tous. On ne sert pas autant les citoyens que les entreprises ?
Et puis j'ai eu un peu de mal avec l'humour de l'auteur. Pour autant, je ne doute asolument des compétences de l'oratricce


La veille techno pour les vieux croutons
-----------------------------------------

_Par Thibault Jouannic_

Un vieux crouton : Persionne qui a laissé ses compétences devenir obsolète.
- Les gens qui n'assument pas trop...
- Les vieux croutons qui assument à mort.
IL FAUT PASSER DU TEMPS à se remettre en question, se maintenir à jour...
Le problème c'est quand la veille techno devient une corvée. C'était devenu chronophage et rébarbatif et pénible.
Quoi faire ? Changer la manière d'appréhender ma veille techno
- Se débarasser de la culpabilité : Facile, utiliser un projet mature c'est gage de stabilité.
- Etre plus efficace : Ne plus se lancer sur un projet perso ; Aller chercher des vrais retour d'expérience. Cibler un peu plus.
- Etre ludique : Pour être fun ça doit être enrichissant. Parfois ca n'a rien à voir. S'ouvrir à d'autre champs.

Finalement le vieux crouton, c'est celui qui ne veut plus apprendre.

_Mon avis :_ Conférence sympa et ludique. Il faut de toute manière que je re-réfléchisse à nouveau comment faire ma veille techno.
Je blogguerais la dessus plus tard.


Bon robots, mauvais robot, un intense traffic
---------------------------------------------

En plus des robots indexeurs, y'a des robots pour trouver les mots de passes, pour cliquer sur les publicités
Il y en a dont on ne connait pas trop l'usage. Ou même des robots oubliés et autres indexeurs fous.
Apparemment, 63 à 80% sont pour les robots. Oo
Les bons robots sont gentils, donc respectent des bonnes pratiques : robots.txt, balise méta, lien nofollow, sitemaps. Les bons robots sont même joignable
Les mauvais robots eux au contraires usurpent leur identité, sont même distribué (se camouflent en utilisant plusieurs IP)
Il existe des API pour connaitre la réputation des adresses IP.
Le [projet Honey pot](http://www.projecthoneypot.org/) cherche à piéger les robots
On peut aussi étudier les en-têtes http : Un chrome qui vient d'une dédibox, qui n'a pas été mis à jour depuis un an et dont l'adresse ip à fait du spam récemment est clairement un suspect.

_Mon avis :_ Une conf très intéressante sur un sujet trop méconnu.



DIY : une console de jeux
-------------------------

L'idée de reprendre un jeu existant, car si l'on veut faire un jeu de A-Z, vous risquez d'être dépassé par la
somme de travail.
Une librairie parmi d'autres : [Phaser](http://www.Phaser.io)
Attention faire les assets graphiques c'est un temps monstre
Repartez d'un projet existant
Jeux à deux : Clavier partagé. Combo clavier souris=Bof. Le mieux c'est le gamepad. marche aussi avec guitare héro. 
Y'a aussi Arduino, pour créer son capteur.
Y'au aussi un controleur qu'on peut acheter qui ne marche pas à la pression mais à la conductité. Chacun porte un pince crocodile,
et quand on se touche la main, une action se produit...
"Passe moi ton téléphone ou ta tablette" disent en les enfants. 


_Mon avis :_ J'ai beaucoup aimé parce que j'avais envie de faire un jeu pour ma filleule. Bon retour d'expérience de la part d'Alvin ( se prononce Alv-un , c'est à dire à la française).



EcmaScript 6 par le code 
-----------------------

_Par Matthieu Lux_


Babel permet de transformer ecmascript6 en ecmascript5
eslint permet de vérifier la syntaxe javascript dans l'éditeur

* on utilise ``let`` plutot que ``var``
* on ajoute des const si je ne modifie pas cette variable
* String : le nouveau séparateur : le backquote
* Le mot-clé Class : sucre syntaxique. Faut quand même comprendre les prototypes et this.
* La fat-arrow function : Se libèrer du mot clé function. Pas seulement sucre syntaxique. C'est un peu déroutant à mon avis. Corrige aussi un problème du ``this`` dont on ne comprends pas ce qu'il contient ou pourquoi son contenu a disparu. Fat Arrow function corrige cela.
* La function anonyme pour faire de l'isolation va devenir obsolète.
* On peut utiliser des modules (mot clés export, import...)
* Les promesses, pour remplacer les callbacks. Permet aussi de faire des chainages (évite l'empilement des callbacks : callback hell). Toutefois normalement vous ne devez pas vous en servir
* Les générators 

Question : Intérêt de ES6 par rapport à CoffeeScript ? Certain innovation en plus de Coffee. Coffee perdra car EmmaScript lui sera apporté par les browsers alors que CoffeeScript est un choix de développeur

_Mon avis :_ Matthieu Lux explique très bien ! J'aimerais bien expliquer comme lui. Impressionnant.


Un outil pour simplifier le debug web sur toutes les plateformes :Vorlon.js
----------------------------------------------------------------------------

_Par David Rousset et Etienne Margraff_

Constat : Le web c'est plus compliqué à debugguer sur mobile, ou sur les objects connectés
[Vorlonjs](http://vorlonjs.io)
cross plateform / cross browser / à distance
8 plugins par défaut

_Mon avis :_ Intéressant, et amusant. La partie démo etait chouette. C'est vrai que débugger sous mobile est compliqué, donc bon outil.


Découper son application monolithique, pourquoi, comment ?
----------------------------------------------------------

_Par Benjamin Fraud , Olivier Dolbeau_

Exemple de bla bla car. Utilise RabbitMQ pour faire des micros services. Un micro service supporte plusieurs versions de format de message interne pour gérer les changements simultané des micro-services
Utilise Chef pour déployer.
Utilise PHP; mais le micro service est aussi l'opportunité de un changement de language de programmation.


_Mon avis :_ Difficile de ne pas adhérer. Retour d'expérience, ne parle pas assez des difficultés, ou des exemples autres que chez BlaBlaCar.
La partie la plus intéressante était les questions ! D'ailleurs la présentation était un peu courte, du coup il y avait beaucoup de place pour les questions. 


Design de soi, valoriser son identité et son expertise sur le web
------------------------------------------------------------------

_Par Marie Guillaumet_

Personnal Branding, mais terme bof, car on n'est pas des marques. Il s'agit d'expliquer ce que l'on fait, pas tant que de se montrer.

Dévoiler ses aspérités...
Dévoiler son expertises, par exemple sa réflexion sur un point technique, son scrapbook mental (ses inspirations), son analyse.
Extimité : à l'inverse d'un journal intime. L'extimité (notion de Michel Tournier) est tourné vers l'extérieur. Paratagez vos rencontres, vos découvertes...
Attention au personnal branling. Ne pas faire d'auto-promotion extrème
En quoi votre métier vous plait ? Quels sont vos points forts ?  
 

_Mon avis :_ Meilleur conf de la dernière journée ? Vivement que je revois la vidéo ! 


Tristan Nitot
-------------

_Mon avis :_ Ah, Je n'ai pas noté ce que Tristan disait. J'adhère tellement à tout ce qu'il dit !
* Retrouvez tout sur son http://standblog.org
* Achetez son bouquin qui sortira prochainement
* Installez un cozycloud comme moi, par exemple sur un raspberry pi 2


La Conf Surprise : Les interprètes LSF
---------------------------------------

Ah que j'aurais aimé voir un Edouard Snowden ou un Tim Berners-Lee lors cette conf surprise. Mais non.
Pourtant cette conférence était super-émouvante. D'abord découvrir la LSF est passionant.
Ensuite découvrir la couverture de la LSF pour Paris-web était génial. 
Sandy, l'oratrice était juste géniale, très drôle ! Dire que c'est sa première conf.
Se rendre compte qu'on ("on" au sens du public autant que les orateurs)  a changé la vie de 
ces traducteurs et converti au numérique, à l'informatique, à la défense de nos libertés sur le web.
C'était très fort. Et malgré tout ce qu'on leur fait subir, terme anglais, private joke, et débit
de parole insoutenable... ces personnes trouvent orateurs et audience géniale, et loue notre bon esprit.



JOUR 3 : ATELIER
================

Quoi faire dans 20 ans ?
------------------------

* Ne pas que regarder ce que je ne sais pas faire sur Internet ! Ne pas oublier aussi ce que je sais faire. Arrêter de se comparer, sinon on va vite tomber en dépression, Internet est tellement immense.
* Il faut faire le boulot qui nous plait aujourd'hui (Eric daspet)
* Au sujet du "Code à l'école" : J'ai fait des maths depuis la maternelle, et c'est pas pour ça que j'ai eu envie d'être mathématicienne.
_Mon avis :_ J'ai échoué un peu à participer; J'avais plus à apporter. J'étais étonné que des jeunes s'inquiètent déjà de cette problèmatique.

 


<a name="conclusion">CONCLUSION :</a>
============

Ah ! Dire que j'ai pu écrire quelques critiques dans ce compte-rendu (c'est même déplacé de ma part), aucune conférence n'était mauvaise ou moyenne ! 
Au contraire, tous les intervenants étaient à l'aise sur scène, tous étaient clairs, tous étaient à l'heure, tous ont su répondre aux questions.
Presque tous avaient des slides clair. Certains étaient super-drôle. 
On s'habitue à l'excellence !
Au niveau du staff, les personnes étaient toujours disponibles, agréable. Tout est si bien rodé : Vestiaire, Amphithéatre, Traiteur avec pièces végétales pour les vegans, sono, traduction, vélotypie (le fait d'écrire de discours de l'orateur en direct), langue des signes, accueil, paiement par carte sur place pour les ateliers... Logement pour les orateurs à coté, review des confs. Vote des informelles.

__Parisweb, c'est une conférence au top__ ! Et je ne parle pas de la __bienveillance__ des gens entre eux : Public, orateurs, organisateurs, prestataires. C'est un miracle, dix fois renouvellé que d'arriver à partager autant d'ondes positives entre nous ! Et de l'humour ? Voir une [licorne faire du hola-hoop](https://instagram.com/p/8UCGN-D00C/?taken-by=hellgy) ou débarquer dans votre atelier ? Fous rires assurés ! 
Et tout le monde bénéficie de ces ondes positives ! Les orateurs ressortent grandis dans leur savoir, les auditeurs enrichis de leur partage, et les organisateurs fiers et auréolés (j'espère) !

Si vous hésitez à aller à Parisweb, vous avez tord !

L'année prochaine, je devrais me positionner. Aider l'évenement à continuer en intégrant le staff ... ?

