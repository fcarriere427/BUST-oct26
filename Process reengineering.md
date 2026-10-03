Je suis consultant chez Wavestone. J'anime un atelier de refonte de processus avec un industriel (fabrication de composants mécaniques). Le processus étudié : le traitement d'une non-conformité qualité en production. Je veux un outil d'atelier qui montre la méthode en trois temps : 1) le processus officiel face au processus réel, 2) le tri de chaque étape réelle en 4 catégories, 3) le processus cible et sa valeur.

Crée une application web dans un seul fichier index.html autonome (HTML, CSS et JavaScript, sans aucune dépendance externe ni appel réseau). Toutes les données sont fictives et codées en dur. Un badge « Données fictives — démonstration » est visible en haut.

TEMPS 1 — « Le processus tel qu'écrit vs tel qu'il est vécu ». Deux colonnes côte à côte.
À gauche, le processus officiel en 7 étapes linéaires : Détection · Déclaration dans l'outil qualité · Analyse · Décision de traitement · Action corrective · Vérification · Clôture.
À droite, le processus réel en 18 étapes, numérotées, avec deux flèches de retour en arrière bien visibles (étapes 6 et 14) :
1. Le chef d'équipe remplit une fiche papier
2. Ressaisie de la fiche dans l'outil qualité le lendemain
3. Photo du défaut envoyée par messagerie au technicien qualité
4. Vérification que la pièce, le lot et l'ordre de fabrication existent
5. Recherche dans un fichier Excel parallèle pour savoir si le défaut est déjà connu
6. Relance par mail du chef d'équipe car il manque des informations (retour à l'étape 2)
7. Classification du défaut (type, gravité)
8. Blocage du lot dans l'ERP si la gravité est majeure
9. Recherche des causes probables dans l'historique
10. Attente de la réunion qualité hebdomadaire
11. Décision : reprise, rebut ou dérogation
12. Si dérogation : accord écrit du client
13. Rédaction du rapport d'analyse 8D
14. Rapport renvoyé par le responsable qualité car incomplet (retour à l'étape 13)
15. Création de l'action corrective dans l'outil
16. Relance des responsables d'actions en retard
17. Vérification de l'efficacité de l'action
18. Mise à jour manuelle du tableau de bord qualité mensuel
Sous les colonnes, trois chiffres choc : « 7 étapes sur le papier, 18 dans la réalité », « 38 % des dossiers repartent en arrière », « 21 jours de délai pour 3 heures de travail effectif ».

TEMPS 2 — « Trier chaque étape ». Chaque étape réelle a 4 boutons de catégorie : Supprimer (gris : l'étape ne devrait plus exister), Règle automatique (bleu : si X alors Y, aucun jugement), Agent IA (vert : demande du jugement et un historique existe), Humain (orange : trop risqué pour se tromper — décision, engagement client, validation). Un compteur par catégorie se met à jour en direct. Un bouton « Voir la proposition de l'expert » applique la proposition suivante et surligne les écarts avec le choix du participant :
Supprimer : 1, 2, 3, 6, 10, 14 · Règle automatique : 4, 8, 15, 16, 18 · Agent IA : 5, 7, 9, 13 · Humain : 11, 12, 17.
Pour chaque étape, une courte justification de la proposition apparaît au survol.

TEMPS 3 — « Le processus cible ». Un bouton « Générer le processus cible » lance une animation : les étapes « Supprimer » s'effacent, les étapes « Règle automatique » se rangent dans une bande « automatisé », les étapes « Agent IA » se regroupent en 2 agents (« Agent de qualification » = 5 et 7 ; « Agent d'analyse et de rapport » = 9 et 13), et les étapes « Humain » restent comme 3 points de contrôle. On obtient un processus cible lisible de 10 blocs. Puis un tableau avant / après apparaît avec des barres animées : nombre d'étapes 18 → 10 ; délai de traitement 21 jours → 6 jours ; dossiers qui repartent en arrière 38 % → 8 % ; coût par non-conformité 640 € → 190 €. En bas, une phrase de conclusion : « L'essentiel du gain vient de la suppression des attentes et des boucles, pas de l'IA seule. »

Navigation : trois onglets ou trois sections numérotées (1, 2, 3), avec un bouton « Étape suivante ».

STYLE — professionnel, type cabinet de conseil : fond violet très profond (#1E1145), cartes plus claires, texte blanc, accent vert néon (#04F06A). Police système sans-serif. Responsive, lisible au vidéoprojecteur.

EXPORT — un bouton « Exporter en PDF » qui lance l'impression du navigateur (window.print), avec une feuille de style d'impression : fond blanc, texte sombre, sans boutons, les trois temps visibles l'un sous l'autre.

QUALITÉ — la page s'ouvre sans erreur dans la console, tous les textes sont en français.