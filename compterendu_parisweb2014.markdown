Title: Compte rendu de Paris Web 2014
Date: 2014-10-24 18:30
Tags: paris-web
Category: paris-web
Author: Cédric Levasseur
Summary: compte-rendu de paris web 2014

Je suis allé une fois de plus à [Parisweb](http://www.parisweb.fr) 2014, la conférence qui promeut les bonnes pratiques du web.

Je ne compte plus les fois (est-ce la cinquième) que j'assiste avec enchantement à cet évênement.
Je suis resté dans l'energie de [SubWeb](http://www.sudweb.fr), c'est à dire aller au devant des gens et discuter avec les personnes,
plutôt que rester timidement dans mon coin comme j'ai l'habitude.
C'était d'autant plus facile que je connaissais pas beaucoup de personne, et que je les suivait sur twitter.
Astuce : Si vous allez à une conférence, essayer de réunir (par twitter) quelques infos sur les personnes , qu'ils soient de l'assistance, du staff ou orateurs.
(Faudrait que je me souvienne de cette astuce)


Je retiens plus un esprit de camaraderie qu'une grosse claque de connaissance technique. Peut-être parce que la conférence a fait le tour des techniques.
Parisweb reste quand même un socle de petite découverte. Et je suis surpris aussi là ou l'on s'y attends le moins.
J'ai raté la conférence de David Rousset, pourtant il m'a donné très envie de faire du TypeScript (un langage au dessus du Javascript).
Egalement raté la conf de Rémy Parmentier (@Htmeuleu), très drôle et intéressante techniquement sur les problèmes d'intégration des newsletters (un rare domaine qui ne s'améliore pas). Petite réflexion : Outlook est-il le IE6 (comprendre : un logiciel boulet) de la newsletter ?

Parmi les conférences que j'ai vu en live :

Qualité web :
-------------
Les outils web se sont améliorés, les métiers se spécialisent et on en fait plus pour moins cher. Il faut donc faire payer la qualité, et pour cela, améliorer son savoir ne suffit, encore faut-il se mettre en avant ! Merci Elie pour ces précieux conseils.

Le web fait pousser mes tomates
-------------------------------
J'ai été abasourdi par la liste de "patchs" (pour reprendre la parabole de l'auteur) que l'industrie agroalimentaire applique pour pratiquer la culture intensive.
Le monde va vraiment pas dans le bon sens.
- Nitrates
- Hybrides courts
- Herbicides
- Engrais
- Fongicides
- Insecticides
- Pollenisation manuelle
Amusant parallèle entre Hacktivisme et Seed-Bombing : Jeté de graines et culture dans les jardins publics.

WebComponents
-------------
Intéressant et amusant, mais difficile à suivre en Anglais.
Je fais le constat que mon HTML5 est loin derrière moi (Je ne pratique pas assez)
Dire que j'ai acheté le bouquin de Bruce et si jamais pratiqué en envirronnement professionnel, ça me met en rogne.

Pompier du code
---------------
Un pompier c'est
- 50% d'entrainement
- 40% de prévention
- 10% d'intervention
à méditer pour progresser techniquement.
"Une idylle peut virer au cauchemar, l'inverse jamais"

Qualité 
-------
Cette conf m'a déçue, car je m'attendais à plus d'exemple. Je n'y ai rien appris.
Ah si, le terme bikeshed : discussion sur la couleur du hangard à vélo, c'est à dire discussion qui ne mène à rien.

Revue de code
-------------
L'auteur apporte une solution technique à un problème organisationnel. (Utiliser les PR de github pour faire de la revue de code)
Intéressant, mais évidement la technique ne peut pas tout : Il faut une équipe soudée, qui communique. 
Cela me met à l'esprit l'importance de la qualité de la communication entre développeurs.

Reverse proxy
-------------
On devrait tous savoir utiliser apache ou nginx !



* Les locaux :
--------------

Le lieu a changé cette année pour le palais brogniard en plein Paris. Les locaux d'IBM à bois-colombes étiaient très chaleureux et reposant. A part le confort vraiment moyen du salon d'honneur et des salles plus éloignées, difficile de reprocher quelque chose.
 
Les folles journées ou les fourberies d'un projet
-------------------------------------------------
Wah, une première conférence très drôle. Commencer avec ce ton décallé est peut être un peu risqué.
Difficile d'apprendre quelque chose de cette parodie de projet néanmoins.
J'en retiens des mécanismes pour mettre la pression :
- Ne pas maîtriser l'environnement technique : "Au fait on utilise Drupal"
- "Je me suis installé derrière le DA" pour être sûr qu'il avance.
- "J'ai demandé à tout le monde, j'ai fait une moyenne" au sujet de la couleur principale du site, ou comment le manque de décision génêre de la frustration, des allers et retours inutiles.

Bonne pratique des APIs, par E.Daspet
-------------------------------------
Comment faire en sorte que les API soient comprises et bien utilisées ?
TOP 5 : 
* prévoir dès à présent l'internationalisation.UTF-8 bien sûr. Mais ne pas utiliser de dates, plutôt des heures (timestamp ?). J'avoue ne pas avoir compris pourquoi.
* pagination : oubliez "offset" + "quantités", trop compliqués à gérer, surtout que votre base peut changer durant un changement de page. Préférez "suivant/précédent". En plus le cache fonctionnera mieux. Pensez vraiment à la pagination dès votre première release. 
* versionnement des APIs. Indispensable d'y penser dès le départ. La rétro-compatibilité des apis sera galère a gérer, mais si vous mettez un numéro de version dans l'url, ca se passera mieux /v01/ ...
* Sécurité : Toujours utiliser Oauth et HTTPS systématiquement. Simple efficace et éprouvé. De plus toujours utiliser une clé d'API. Fournir une clé d'API à ceux qui utilisent vos API va vous permettre se savoir qui fait la requête qui plombe votre serveur :)
* Structure d'URL :  De toute manière les utilisateurs bidouilleront vos URLs, dont faites simple et compréhensible. 3 profondeurs maxi dans l'URL, des minusucules, pas de caractères spéciaux.

Au final une bonne conférence technique simple efficace et pratique !
Je pense qu'elle me servira pour faire mes Webapps, même si je ne fait pas (encore) d'APIs.

Je code donc je teste :
-----------------------
- C'est le processus que l'on va mettre en place qui va apporter de la qualité, pas tout à fait le fait de tester !
- Oubliez les alerts/printf/log. pour développer, débuggez avec les outils modernes.
- Il existe des frameworks de test pour les tests unitaires, les test d'intégration, les tests fonctionnels
- Si vous ne faites pas encore de tests, restez réalistes, commencez simple, par des tests unitaires et des résolutions de bugs.
- Il existe Sélénium, mais aussi Sikuli pour des tests fonctionnels.
- Mais au final TOUJOURS tester.

Cette conférence était une bonne piqure de rappel.

Construisez vos API :
---------------------

- Les singes en groupe oublient pourquoi ils transmettent des règles qui les protégaient de l'eau glaçée, longtemps après que le danger soit terminé. Nous aussi :) N'oublions pas de nous remettre en question, d'essayer, de tester.
- Utiliser les mêmes stacks d'outils pour tous crée aussi des problèmes, la diversité c'est bien aussi.
- N'ouvez vos API que petit à petit, pas trop d'un coup.
- restez cohérent (dans les paramètres de fonctions) et documentez.
- Standards, standards, standards..
- Utilisez les codes de retour HTTP !
- Développez c'est bien ! MAIS DIFFUSEZ LE !!!
- faites du static dès que possible.
- Dans votre boite à outils : microjs.com / sass, less / jekyll, kinby, pelican / grunt, rake
- Aujourd'hui le web se builde (contrairement au tout dynamique d'hier)
- "Le web est et restera un métier d'artisans passionnés"

Au final une conférence bien intéressante, avec du bon sens. 

Les 7 préceptes d'un projet raté :
----------------------------------
L'objectif de cette conférence est d'échouer :)
- "La communication verticale devient téléphone arabe"
- Les outils qui deviennent torture
- Les méthodes qui deviennent effet tunnel
- On a toujours tendance à penser que l'expérience raté est de la faute du client


Goût et mauvais goût :
----------------------

"Les goûts sont subjectifs, ne se discutent pas..." Vraiment ?
Le design n'est pas une affaire de goût.
- L'esthétique : Quelle tête aura ce que je vais mettre au monde ?
- On ne peut pas ne jamais tenir compte de l'esthétique, du design.
- Si tous les goûts se justifient, alors aucun n'est justifié ! 
- Il s'agit donc d'une réaction emmotionnelle.
- Le design a pourtant bien une utilité !
- (Apple s'est inspiré de Dieter Rams (qui travaillait chez Braum)
- "Goût" vient du latin "Gus" qui signifie essayer.
- Les produits affectent notre bien être.
- Le goût est relatif 1: aux cultures 2:aux époques 3:à notre expérience personnelle.
- Quelques lois : 
	* le nombre d'or (1,618)  
	* la loi de gestalt (loi de proximité et/ou loi de similitude)
	* règle des tiers (ex en photographie). (moi ça me fait penser à mon pliage de serviette de bain que je préfère plié en 3 dans l'armoire :) )
	* aussi : loi de Hicks, de Fitts, de Paretto.
	* Mais ces lois ne sont pas des dogmes !
- Beau design est différent de bien fait.
- La typographique apporte de l'organisation dans les lettres et ça donne envie de lire.
- Développer votre culture visuelle et connaissez les références.
- Le mauvais goût vient : d'une mauvaise exécution / en décallage avec notre époque / en décallage avec le contexte / d'une atteinte à notre vécu.
- Mais le mauvais goût peut aussi s'érriger en second degrès ou outil de transgression.
- Attention bon gout d'aujourd'hui est le mauvais goût de demain. Peut-être sera-t-il la tendance de demain. 

J'ai trouvé cet orateur talentueux, c'était passionant.
 
Sécurité, deux ou trois choses que vous ne savez pas :
------------------------------------------------------

- Parmis les attaques connues : XSS, CSPF, Injection SQL.
- Pensez aux mises à jours des CMS, prévoyez les dans les contrats !
- car Il existe d'autres attaques possibles : dénis de service (Dos) / SynFlood / Certificat

- Pourquoi m'attaquerais-t-on, moi ? pour le fric, la politique, l'amusement vandaliste, ou une démonstration de piratage. Par hasard ou dommage collatéral !
On peut louer des services d'attaque par Dénis de service (par irc, en bitcoins :) "Crime as a Service")
- La sécurité informatique doit faire appel à d'autres réactions que la panique primaire ou l'aveugement d'une autruche ! Il faut se méfier de nos intuitions.
La sécurité d'une chambre ou l'on publie ses photos facebook est en contraste avec la visibilité publique et Intemporelle d'Internet.
- La sécurité est poluée par des fausses idées délirantes, des amateurs ignorants !
- Vous devez avoir une supervision de votre système !
- Le Dos consiste à mettre DOWN un site par attaque volumétrique ou par faille.
- Le Syn Flood : consiste à ouvrir des sockets en masses et ne pas transmettre d'accusé de reception. 
- Le Flash Crowd (code de retour HTTP: 429 Too many request) est soi une attaque de botnet soit légitime : être Slashdotté.
- Il faut surveillé.
- Souvent on réagit quand c'est déjà trop tard.
- Vous pouvez utiliser HTtrack pour générer une image statique de votre site qui palliera à l'attaque 
- Mais dans tous les cas, il faut se préparer à l'avance.
- DNS : est souvent le maillon faible. On ne pense par à répliquer les serveur DNS.
- On pirate même les registres (le .my)
- L'empoisonnement DNS est finalement très rare.
- DNSSec permet de signer les noms de domaines.
- HTTPS garantit
	* que je parle au bon site
	* aucun méchant ne m'écoute
- Mais si HTTPS est vérifié par les autorités de certifications X509, il y en a 900. Et ils peuvent certifier que vous parlez bien à la mafia ! 
- En résumé : 
	* La sécurité n'est pas un produit mais un processus.
	* Il faut se préparer et planifier à l'avancer
	* Il faut se coordonner et communiquer.
	* Et aussi : diversifier votre infrastructure et eduquez-vous


Webapps et site web, le jeu des différences :
---------------------------------------------

(A noter : Il ne faut pas prendre webapps au sens seulement d'application web comme "java". Il s'agit aussi des App mobiles...)
Similitudes : DNS, URL, HTML
Historique des navigateurs : en 1991 finalement le web n'était qu'une liseuse HTML. ( :) )
1995 : Netscape insère javascript
1998 : IE ajout XHR (Ajax)
2013 : Environnement application
Désormais on peut faire du 
* stockage (Storage ou IndexedDb), gérer l'Offline, Application Cache.
* graphisme : canvas, webGL, css3 et +
* Maitriser l'environnement : géolocalisation, batterie, file API.
* On peut faire communiquer deux "sites" ensemble.

En conclusion il faut gérer les webapps comme des sites web ! (ou inversement)

Hacktivisme et société civile : un enjeu pour les libertés numériques :
-----------------------------------------------------------------------
En vrac :
* La France un pays sous surveillance, vend ses technos pour surveiller les peuples (Amésis)
* Hadopi bientôt intégré au CSA
* Internet des objets : bientôt plus d'objet en ligne que d'humain ? Qui décide des traces laissés par les objets ?
* Laurent Chemla : "Je vous ai menti".
* Hacktivisme : communauté avec un éthique (libre accès, libre info, décentralisation et joie d'apprendre). Cf l'éthique des Hackers de Stephen Levy, paru en mars en Français, et sur le stand d'Eyrolles à Paris-web.
* Déclaration d'indépendance du cyberespace
* Hacktivisme : comprendre et hacker les processus politiques.
* "Vie privée pour le pauvre, transparence pour le puissant"
* Au final tout est politique (Enjeux sociaux, liberté, outils, place de l'utilisateur : acteur ou consommateur)


Mon avis : Beaucoup de chose lors de cette conférence de qualité par une journaliste, toutefois j'étais au courant de tout cela, ce qui m'intérroge presque sur la qualité de l'information que j'ai su constitué au cours de ma veille perso. Je devrais quand même plus m'impliquer.

Le web après les mots de passes :
---------------------------------

* Trop de gens utilisent le même mot de passe pour tous les services, et trop simple.
* On constitue des bases de données de mot de passes de plus en plus !
* Ne pas utiliser le même mot de passe pour votre boite mail que pour vos autres comptes. Car si votre compte est hacké, ce qui vous authentifie est votre email !
* Une authentification forte, c'est deux parmi :
	- ce que l'on sait
	- ce que l'on a (mobile, dongle,...)
	- ce que l'on est (biométrie)
* OTP = One Time Password.
* Carte à puce : contient un PKI, génère un cryptogramme avec un challenge (=random) émis par un serveur.
* Mobile : Authentification 2 ways, qui réalise une opération chrypto.
* La sécurité, un compromis entre Sureté, Bon marché, rapidité de mise en oeuvre.
* Le login social : Un seul identifiant et un nouveau mot de passe, mais risque pour la vie privée, et attention au partage de données privées.
* Parmi les protocoles de délégation :
	- OpenID depuis 2005 mais en perte de vitesse (google, yahoo, orange, wordpress)
	- BrowserID = mozilla persona. Identifiant = email. Pas mal de bridge.
	- Oasis saml
	- OAuth : le plus utilisé. Mais il fournit des autorisations aux applis tierces. Il faut avoir conscience que l'appli peut connaitre vos followers twitter par exemple.
	- OpenID Connect : Se base sur OAuth, mais limite à juste l'identité de l'utilisateur.
La conclusion du conférencier : Les mots de passe c'est mal, pas pratique, utiliser un authentificateur délégué.

Mon avis : Conf intéressante (parfois un peu molle) mais dont la conlusion va à mon avis à contre-courant de ce qui nous est présenté. Je pense qu'il ne faut surtout pas faire confiance à un tiers pour stocker son mot de passe et j'aimerais héberger mon autorité de délégation personnel. Finalement les gens se font leur Single-Sign-On perso en utilisant le même mot de passe. Je continue de réfléchir sur la politique que j'applique sur les mots de passes, choses que tout le monde devrait reconsidérer.

A noter : Stéphane Bortzmeyer a fait remarque au conférencier qu'il avait oublié de mentionner X509 (TLS)

L'intégration, ce monde du « ça dépend » par Nicolas Hoffmann :
---------------------------------------------------------------
* "Ce n'est pas parce que [ les multiples évaluations de l'intégration lors de l'énoncé du cahier des charges ] est inconsciente, qu'elle n'existe pas"
* L'intégration est un compromis entre : Le support d'IE / Le cadre du projet / La demande expresse du client / L'équipe et les saisisseurs du contenu.

Mon avis : Une conf sympa, et amusante.

Boucles de rétroactions, ou comment personnaliser vos applications par Florian Le Goff :
---------------------------------------------------------------------------------------- 
* Exemple d'amazon ou les actions faites sur le site aident à déterminer nos actions futures (livres achetés, consultés, dernières adresses. aussi : date et heure et device de connection)
* quelques outils :(api de sms : lexmo ?), google production api, apache mahout (basé sur hadoop), kiss metrix, mixpanel.
* Calculez, expérimentez, vérifiez les hypothèses et scénari.
* Mais n'effrayez pas vos clients : Ne dévoilez pas au père d'une ado qu'elle est enceinte !

Livre électronique et standards du web, par Daniel Glazman :
------------------------------------------------------------
Book vient éthymologiquement de l'écorce du hêtre. On écrit toujours sur de la cellulose.
Historique : 1971 : Projet guttemberg. 1992 : première liseuse (Softpress). 1998 cytale. Depuis 2005 : kindle, kobo et nook. Puis ipad.
Dès la première liseuse, ça ressemble fort à du web.
Premier standard en 1999, OpenEbook, basé sur xhtml. Aucun outil d'Authoring.
Epub2 (parti depuis OpenEbook) : xhtml1.1 (on préfère le xml dans l'édition). Pas de Javascript, ni MathML, ni vectoriel, trop nombreuses Tables des matières. des fontes peuvent être embarqués avec obfuscation.
ePub3 : trop vite spécifié. XML toujours, nouvelles méta-données, support de CSS3, MathML, possibilité de désactiver le reflow (exemple des poésies), Media Overlay = viewer spécifique, livres sonores.La spec est incohérente, et pas de suite de tests !
Basé sur HTML5 non finalisé.
Problème : un site peut se mettre plus à jour qu'un eBook.

Calibre, un logiciel bien pratique mais au code "épouvantable".
Une alternative lancée par Daniel Glazman, E0 (google group) avec Dave Cramer (Hachette Livre)

 
Keep calm and carry on par Lou Schwartz :
-----------------------------------------
La conférencière nous raconte comment elle a aidé sa stagiaire a modérer son problème de stress.
Dans un premier temps, on essaie les solutions classiques : Echange, on tente de rassurer la personne. Puis on essaie d'encadrer plus, d'étailler les tâches. Ces solutions sont restés sans effets.
Rien de tout cela n'a marché, et le stress d'un stagiaire se contaminait au reste de l'équipe !
- Accepter la limite de travail que je peu faire par jour. A l'aide de Légo, quantifier la somme de travail effectué et la somme restant à faire !
- Identifier les moments d'augmentation du stress. Tracer un graphique retraçant son niveau de stress acceptable au cours des derniers mois. Y indiquer évenements professionnel et personnel. 
- Au final, réaliser que l'on trouve soi-même ses solutions.
Conclusion : Le stress est souvent un problème de (manque de) communication. Il s'agit aussi parfois d'une mauvaise perception entre l'immaginaire et la réalité. (Bien sur il existe aussi du stress légitime.)
Quelqu'un du public fait le parallèle avec les méthodes agiles qui aident à quantifier et relativiser. "Rester humain, rester serein".

Mon avis : Incroyable que Lou soit  personne allée aussi loin pour aider quelqu'un. Je n'aurais pas imaginer que l'on apporte un jeu de Légo en entreprise et lui demander de "construire" durant ses heures de travail. Je suis admiratif, je pense que j'aurai laissé tomber la stagiaire. J'en retiens que j'ai beaucoup a apprendre en management et en communication. Et aussi nous sommes responsable aussi du niveau de stress que nous nous mettons, et que nous avons la capacité de le contrôller, au moins partiellement.

Les méthodes d'influences sur le web :
--------------------------------------
Parmi les méthodes d'influence d'un site web :
- L'ordre d'apparition dans Google
- Un nom de site simple
- L'apparence : un beau look
- Attention, trop de choix tue le choix.
- Des photos qui utilise le cerveau reptilien : présentant de la Nourriture, un caractère sexué, ou une menace.
- Les commentaires, éléments de rareté (promo, petit stock...), élements de confiance (vote, commentaires clients...)
- Une étique ? On peut influencer de manière maveillante (agir contre la volonté du client)  ou bienveillante (aider à choisir).

Mon avis : C'est à nous en tant que consommateur de faire attention à ne pas nous laissez trop influencé. Avec l'habitude, le nibre arbitre revient, mais c'est aussi une question de discernement et d'éducation, et il ne faut pas trop négliger ces influences. Evidemment il n'y a pas que sur le web que l'on se laisse influencer.
Une parenthèse
Cela me rappelle les toilettes de la gare Saint-Lazare ! Je m'explique : Dans les urinoirs est désinné une mouche sencé aidé à viser le centre de l'urinoir. Je ne sais pas ce que je trouve choquant : Que l'on m'influence à ce moment-là, ou que l'on fasse passer qu'uriner sur un animal soit amusant pour les autres hommes. Je trouve que dessiné un cible de flechette aurait été plus drôle, moins choquant. Bref l'influence ne marche par pareil pour tous, car mon ressenti aurait été d'éviter la mouche ! 

 
Appartheid : Cette conférence était présenté par quelqu'un de chez Ekino. J'ai passé l'année dernière un entretien de recrutement horrible chez eux. Les circonstances étaient particulières : un jour d'hivers ou la neige surprend tout le monde : tous s'inquiètent de rentrer chez soi, Je pense que ni moi ni la recrutrice n'avait envie de rentrer tard chez nous. Ma candidature a été expédiée ! Les question que je posais ne trouvaient que des réponses racourcient sur un ton méprisant. "Tout Ekino va à Paris-Web, évidemment !". J'ai croisé trois personnes, c'est vrai. Je ne m'étais jamais senti si  mal en sortant d'un entretien, je suppose que c'est un test de recrutement. J'ai demandé des excuses à la recrutrice. Cela aurait intérogé n'importe quelle personne sur son processus de recrutement. Elle m'a répondu que ma "Candidature n'était pas retenu". Désagréable jusqu'au bout et c'est fait exprès. Ekino, une entreprise a éviter absolument !!!

Esthétique et pratique du Web qui rouille par Olivier Thereaux et Karl Dubost :
-------------------------------------------------------------------------------
Un ticket de caisse, comme on en a tous dans nos poches. On peut le jeter. On peut le conserver comme preuve d'achat pour quelques jours. On peut le garder pour garantie, durant un ou deux ans. Et puis on peut le garder définitivement, pour mémoire, par garder l'historique des passages dans les lieux, car l'adresse est indiquée dessus.
On appelle cela de l'infobésité, le principe de garder de l'information jetable. Et même si beaucoup pensent qu'il y a trop d'informations, nous avons désormais la capacité de conserver l'information pour se souvenir, pas forcément pour archiver. Pourquoi effacer ? On ne maitrise pas toujours l'effacement. Ainsi un égyptien n'avait pas prévu de garder la stelle d'exonération d'impot si longtemps, mais elle nous a permis de décrypter les hiéroglyphes. On peut comme David Larlet effacer ses tweets qui ne représente pour l'auteur que la pensée du jour, ou l'on peut en faire un carnet de vie. 
On efface parfois en nous méprennant de la valeur. Ainsi le CERN avait fermé la première page web, mais un collectif l'a réouvert pour ses 20 ans ! C'est d'autant plus dur de jeter l'ancien. Jeter une pub actuelle, c'est facile, mais une pub d'il y a 60 ans a pris de la valeur !
Alors, préserver le web ? Comment faire ?
- Mettre des dates dans les URLs
- Utiliser des boîtes à outils.
- Utiliser les bon codes de redirection HTTP (temporaire pour maintenance / permanente).
- Etre techno-opaque : .php ? .html ? ca ne sert à rien ces extensions et poseront problème lors de refonte. 
- Utiliser les bons codes d'erreurs HTTP : 404 -> ? Utiliser aussi 410 : Gone.
- le SEO : robots.txt permet de ne pas référencer l'ancien au profit du nouveau.
- Attention aux pages qui ne sont pas datées ! Elle seront un jour obsolète et erronée si non datées. Toujours indiquer : écrit le.., mis à jour le... 
- Finalement on commence à comprendre la matériau web.
- Question de la vie privée, de l'éthique de ne jamais effacer. Pourtant, on n'efface jamais sa mémoire.
- Question : Conserver les web-applications ? Au moins l'info perninente mérite d'historisée. Par exemple les organigrammes.

Mon avis : Effectivement on ne pense pas assez à la pérénité de l'information sur Internet, car nous ne sommes pas encore habitués à voyager dans le temps. Rien de plus irritant de lire une information impossible à dater. Quid du versionning des pages web, de l'historisation des pages. Très peu de solution pratique. Le mieux est souvent de rendre statique (statufier ?) les pages. Pourquoi pas un module apache-git qui versonnerait les pages web ?

Designing with Sensors: Creating Adaptive Experiences par Avi Itzkovitch :
--------------------------------------------------------------------------

Une conférence ou j'ai fais l'expérience de ne pas prendre de notes et de me laisser bercer par l'orateur.
Mon avis, en anglais pour transmettre à l'Auteur :
I enjoyed this conference. I was surprized of all theses comment about the fear of being influenced by crossing information. I also think it's a little scary to be woke-up earlier by a computer due a subway failure. (I think it's more important to sleep longer and work less, but it's a choice i have :) ) Some complains about having a life over-organized by a computer. Other complains we'll become unhumans. A computer is not able to predict us to fall in love, so life will be enjoyable, as long as it will be. A computer is not able to choose for us, so we will stay humans. In every little thing human does, it's more and more technical. From engineering to Art or Sports, everything is more technical than ever. We are in the over-technical century ! So we shouldn't be afraid to progress as human being. We shouldn't be afraid to process more and more information and used it, by crossing it. Of course, the ethic problem need to be solded, as always. But i don't share the global opinion of fear. We need to learn what's good and evil and preserv ourself. But we should accept to progress !

Mobile et accessibilité, une partie à Troie par Goulven Champenois :
--------------------------------------------------------------------
- 72 % des handicapés utilisent la synthèse vocale de leur smartphone.
- Tout le monde utilise une télécommande pour sa télé : Elle était prévue au départ pour les handicapés ! (hum ?)
- "Les smartphones font de nous des handicapés du web !" : pas de souris, d'écran large, de flash, de clavier, parfois pas de connection et pas d'autonomie :)
- Accessibilité (alt, contraste, pop-in, background)
- Opérabilité (no hover, iframe et scrolling, temps de session, stockage local)
- Compréhensible (langue, abbr, étiquette, ordre du code source)
- Robustesse (validité html, import adaptés, pages allégées, responsive mais bien fait !)
- Au final : Le mobile est le prétexte de la refonte pour rendre enfin nos pages accessible !

Le paradoxe du choix par Anne Lacan :
-------------------------------------

Nos utilisateurs de site web peuvent être embêttés par trop de choix.
Dans tous les domaines de la vie (amour, travail, consommation, ...) le choix nous submerge.
Est-on plus heureux d'avoir le choix ?
En tout cas, il peut en résulter :
- Paralysie,
- Insatisfaction (avoir le meilleur),
- Culpabilité.
Comment choisit-on : On définit un objectif principal, puis une liste que l'on priorise, que l'on évalue.
Il faut donc permettre à l'utilisateur de chercher, de filtrer, lister les options et stocker (wish-list ou panier). 
Attention donc : à ne pas frustrer l'utilisateur, en proposant un autre produit juste avant qu'il passe commande !

Mon avis : conf intéressante et drôle. Jeune, talentueuse, jolie et drôle. C'en est frustrant !  
