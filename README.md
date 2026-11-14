IT LAB – Interactive Learning Platform

Plateforme pédagogique interactive pour les travaux pratiques de l'Atelier Technologies WAN : cours, démonstrations, console de commandes, simulateurs, quiz et suivi de progression.

Auteure : Lina Ben Alaya · Classe : RSI31 · Établissement : ISET Nabeul


Sommaire
Présentation
Contenu
Les cinq modes
Simulateurs calculés
Fonctionnalités
Utilisation
Structure du projet
Intégrer une simulation ActivePresenter
Limites
Feuille de route
Présentation

IT LAB transforme dix énoncés de TP en parcours d'apprentissage. Au lieu de lire un compte rendu, l'étudiant comprend la théorie, observe la manipulation, la refait lui-même, s'évalue, puis consulte la correction.

Contenu

Dix TP, regroupés en cinq thèmes.

Thème	TP	Outil
Cœur de réseau MPLS	TP1 partie 1 – Backbone MPLS : OSPF et EIGRP	GNS3
Cœur de réseau MPLS	TP1 partie 2 – Activation de MPLS et LDP	GNS3
Cœur de réseau MPLS	TP2 – VPN MPLS pour un client	GNS3, Wireshark
Routage entre domaines	Lab BGP – eBGP entre deux fournisseurs	Routeurs 1841 ou GNS3
Routage entre domaines	TP Redistribution – OSPF, EIGRP et RIPv2	GNS3
Services IP	TP3 – DHCP et NAT	Packet Tracer
VPN chiffrés	TP5 – VPN IPsec site à site	GNS3, Wireshark
VPN chiffrés	TP5 bis – Tunnel GRE over IPsec	GNS3, Wireshark
Frame Relay	TP6 – Frame Relay de base	GNS3, Wireshark
Frame Relay	TP6 bis – Frame Relay avancé, hub and spoke	GNS3, VPCS

En chiffres : 10 TP, 118 commandes à saisir, 40 questions de quiz, 5 simulateurs.

Les cinq modes
Mode	Ce que fait l'étudiant
1 · Apprendre	Lit les objectifs, les notions clés, la topologie et l'adressage
2 · Observer	Regarde les commandes de la manipulation rejouées pas à pas
3 · Pratiquer	Saisit les commandes IOS dans une console, avec indices et validation
4 · Évaluer	Répond à un quiz noté, sans aide
5 · Corriger	Consulte la réponse attendue et l'explication de chaque erreur
Simulateurs calculés

Chaque simulateur recalcule son résultat quand on change un paramètre.

Simulateur	TP	Ce qu'on manipule
Table de traduction NAT	TP3	Mode statique, pool ou surcharge ; nombre d'hôtes
Trajet d'un paquet labélisé	TP1 partie 2, TP2	Service (backbone ou VPN), sens du trafic
Distance administrative	TP Redistribution	Distance des routes EIGRP externes
En-têtes GRE et IPsec	TP5, TP5 bis	Type de tunnel
Panne d'un PVC Frame Relay	TP6 bis	Interface multipoint ou sous-interfaces, état du PVC
Fonctionnalités
Tableau de bord : avancement par TP et par mode, score moyen, activité conseillée
Mode défi : dix questions aléatoires en trois minutes
Recherche dans les TP, y compris par commande (show mpls, overload…)
Glossaire technique relié aux TP
Thèmes clair et sombre
Interface adaptée au mobile et utilisable au clavier
Utilisation

Le site tient dans un seul fichier, sans installation ni serveur.

En ligne : ouvrir le lien de démonstration.
file:///C:/Users/PC/Downloads/IT%20LAB%20%E2%80%93%20Lina%20Ben%20Alaya,%20RSI31.html#accueil

En local :

bash

cd it-lab
voici le lien du LAB : file:///C:/Users/PC/Downloads/IT%20LAB%20%E2%80%93%20Lina%20Ben%20Alaya,%20RSI31.html#tp-tp1a
Puis ouvrir index.html dans un navigateur.

Publication sur GitHub Pages :

Déposer index.html à la racine du dépôt.
Ouvrir Settings › Pages.
Choisir la branche main et le dossier / (root), puis enregistrer.
Le site est disponible après une à deux minutes.
Structure du projet
it-lab/
├── index.html    Le site complet : styles, données des TP et code
└── README.md

Dans index.html, le contenu des TP est regroupé dans le tableau TPS. Chaque TP contient :

Champ	Contenu
obj	Objectifs
topo	Topologie et adressage
no	Notions : terme et définition
st	Étapes : invite, commande attendue, explication
qz	Quiz : question, quatre choix, bonne réponse, explication

Ajouter ou corriger un TP revient à modifier ce tableau.

Intégrer une simulation ActivePresenter



Limites
Aucune commande n'est exécutée sur un équipement réel : la console compare la saisie à la commande de l'énoncé.
Les simulateurs sont des modèles simplifiés ; leurs hypothèses sont affichées à l'écran.
La progression est enregistrée dans le navigateur de l'utilisateur, sans synchronisation entre appareils.
Les démonstrations du mode Observer sont reconstituées à partir des énoncés, en attendant les exports ActivePresenter.
Feuille de route
[ ] Exports ActivePresenter des dix manipulations
[ ] Schémas de topologie interactifs
[ ] Comptes rendus au format PDF
[ ] Simulateurs « annonces BGP » et « import de routes VPN »
[ ] Attestation de fin de parcours

Projet réalisé dans le cadre de l'Atelier Technologies WAN, ISET Nabeul.
