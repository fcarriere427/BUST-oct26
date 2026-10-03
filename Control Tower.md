Je suis consultant chez Wavestone. Demain, j'anime un atelier avec la direction d'un gestionnaire d'infrastructures de transport (réseau autoroutier : péages, maintenance, viabilité hivernale, centres d'exploitation). Le sujet : piloter la valeur de leur portefeuille de cas d'usage IA, au-delà des POC. Je veux leur montrer en direct à quoi ressemblerait leur « tour de contrôle de la valeur IA ».



Crée une application web dans un seul fichier index-control-tower.html autonome (HTML, CSS et JavaScript, sans aucune dépendance externe, sans bibliothèque, sans appel réseau). Tous les graphiques sont dessinés en SVG à la main. Toutes les données sont fictives et codées en dur dans le fichier.



CONTENU — un portefeuille de 8 cas d'usage IA, chacun avec : nom, domaine métier, étape actuelle, sponsor (un intitulé de poste, jamais un nom de personne), valeur annuelle visée en k€, valeur réalisée à date en k€, taux d'adoption (% d'utilisateurs cibles actifs), coût de fonctionnement mensuel IA en k€ (FinOps), statut (en avance / dans les clous / en dérive / à arrêter), et un commentaire d'une phrase.

Les 8 cas d'usage :

1\. Détection automatique des incidents sur vidéo (centres d'exploitation)

2\. Maintenance prédictive des équipements de péage

3\. Prévision de trafic et d'affluence en temps réel

4\. Optimisation des tournées de viabilité hivernale (salage, déneigement)

5\. Assistant IA pour les agents de patrouille (procédures, consignes)

6\. Analyse automatique de l'état des chaussées par images

7\. Agent de traitement des réclamations clients

8\. Assistant de rédaction des comptes rendus d'intervention

Répartis-les de façon réaliste sur les étapes de la chaîne de valeur IA, dans cet ordre : Stratégie → Cadrage → Construction → Gouvernance → Déploiement → Captation de la valeur. Au moins un cas doit être « en dérive » (forte valeur visée, faible adoption) et un cas « à arrêter » (coût IA supérieur à la valeur réalisée).



ÉCRAN — une seule page, dans cet ordre :

1\. Bandeau : titre « Tour de contrôle de la valeur IA », sous-titre « Gestionnaire d'infrastructures de transport — portefeuille IA », et un badge visible « Données fictives — démonstration ».

2\. Quatre indicateurs clés en grandes tuiles, avec un compteur animé au chargement : valeur visée totale, valeur réalisée totale (et % de la cible), adoption moyenne, coût IA annuel total avec le ratio valeur réalisée / coût.

3\. Une frise horizontale des 6 étapes de la chaîne de valeur (flèches chevrons ; le texte de chaque étape doit tenir dans sa flèche, avec un retour à la ligne si besoin), avec sous chaque étape des pastilles représentant les cas d'usage qui s'y trouvent (couleur selon le statut). Survoler une pastille affiche le nom du cas.

4\. Un graphique en courbes : valeur cumulée visée vs réalisée, mois par mois sur les 12 derniers mois. La trajectoire visée répartit linéairement la valeur annuelle visée sur 12 mois ; la courbe réalisée monte progressivement et atteint exactement la valeur réalisée totale au 12e mois.

5\. Un graphique à bulles : axe horizontal = adoption (seuil à 50 %), axe vertical = valeur réalisée (seuil à 400 k€) ; un cas = une bulle, taille = coût IA, couleur = statut. Quadrants légendés : en haut à droite « Pépites » (valeur et adoption fortes), en haut à gauche « À diffuser » (de la valeur mais peu d'utilisateurs), en bas à droite « À questionner » (utilisé mais peu de valeur), en bas à gauche « À relancer ou arrêter ». Les légendes ne doivent pas être masquées par les bulles.

6\. Un tableau des 8 cas d'usage, triable en cliquant sur les en-têtes de colonnes, avec une barre de progression valeur réalisée / visée.

7\. Un panneau latéral qui s'ouvre quand on clique sur un cas (dans le tableau, la frise ou le graphique à bulles) : toutes ses informations, sa mini-courbe de valeur, son commentaire, et une recommandation d'une phrase (accélérer, corriger l'adoption, ou arrêter).

Au-dessus du tableau : des filtres par statut et par étape, qui mettent à jour tous les graphiques et les indicateurs.



STYLE — sobre et professionnel, type cabinet de conseil : fond violet très profond (#1E1145), cartes légèrement plus claires, texte blanc, accent vert néon (#04F06A) pour les valeurs positives et les éléments actifs, orange pour « en dérive », rouge doux pour « à arrêter ». Police système sans-serif. Animations discrètes (apparition des cartes, croissance des courbes). Responsive : lisible sur un écran de vidéoprojecteur comme sur un portable.



EXPORT — un bouton « Exporter en PDF » en haut à droite, qui lance l'impression du navigateur (window.print). Prévois une feuille de style d'impression : fond blanc, texte sombre (y compris tous les textes des graphiques), pas de boutons ni de filtres, pas d'animation, graphiques conservés, 2 pages A4 paysage au maximum (indicateurs, frise et graphiques sur la première, tableau sur la seconde), et le badge « Données fictives » toujours visible.



QUALITÉ — vérifie que la page s'ouvre sans erreur dans la console, que les totaux des indicateurs sont cohérents avec le tableau, et que tous les textes sont en français.

