# La CAN (Compagnie Alsacienne de Navigation)

Projet réalisé en trinôme, dans le cadre de ma première année de BUT informatique.

## Présentation

La CAN est une compagnie maritime (fictive) qui assure des liaisons entre le continent et les îles de Bretagne : **Lorient ⇄ Port-Tudy (Groix)** et **Quiberon ⇄ Le Palais (Belle-Île)**.

Le site permet aux clients ayant réservé un trajet de visualiser leur carte d'embarquement et leur facture ainsi que de consulter différentes informations sur les liaisons. 

Toutes les données étaient récupérées en temps réel depuis une API mise en place par l'IUT. Malheureusement, l'API est aujourd'hui fermée, mais vous pourrez trouver un rendu du visuel prévu dans la section **Captures d'écran** plus bas.

## Fonctionnalités

- **Accueil** : Présentation de la compagnie, vidéo de Groix, téléchargement de l'application CAN (cette application a été développé par les deux autres membres de mon équipe ! Elle permet de créer une nouvelle réservation).

- **Cartes d'embarquement** : À partir d'un numéro de réservation, génère une carte d'embarquement par passager, par véhicule et par animal. On passe de l'une à l'autre avec les flèches ❮ ❯.

- **Facture** : Calcule et affiche la facture détaillée d'une réservation : catégories de passagers et de véhicules, prix unitaires selon le trajet, totaux.

- **Tableau de bord** : Taux de remplissage d'une liaison à une date donnée, pour chaque horaire.

- **Statistiques** : Chiffre d'affaires et nombre de passagers et de véhicules pour les 4 liaisons, avec le total général, pour Novembre 2025.

## Captures d'écran

- ### Accueil
<img width="2880" height="1466" alt="image" src="https://github.com/user-attachments/assets/d91c5522-ebbc-468b-99e5-3c86aed1a256" />
<img width="2880" height="1466" alt="image" src="https://github.com/user-attachments/assets/f4c0a48e-f9e5-431f-ae69-1caae05455b5" />

---
- ### Cartes d'embarquement
<img width="2880" height="1464" alt="image" src="https://github.com/user-attachments/assets/8a11e041-cb01-46ba-ba20-d6d8bd51695c" />
<img width="2880" height="1462" alt="image" src="https://github.com/user-attachments/assets/97040f9b-1c37-41db-8fec-5ef11283a5f6" />

---
- ### Facture
<img width="2876" height="1462" alt="image" src="https://github.com/user-attachments/assets/9ef624ba-0f5d-48a6-a780-125b66b7bfef" />
<img width="2880" height="1464" alt="image" src="https://github.com/user-attachments/assets/b134f5bd-95a8-4a94-abd2-18a2a83f174d" />

---
- ### Remplissage des liaisons
<img width="2880" height="1466" alt="image" src="https://github.com/user-attachments/assets/44ad9ecb-f9ff-4b36-871c-9b49feb54166" />
<img width="2880" height="1466" alt="image" src="https://github.com/user-attachments/assets/6dad8cdf-e507-4a43-a98b-e88f9ea01178" />

---
- ### Statistiques
<img width="2880" height="1466" alt="image" src="https://github.com/user-attachments/assets/a3a4db8c-a0b5-47a2-885e-dd12d35583db" />
<img width="2880" height="1468" alt="image" src="https://github.com/user-attachments/assets/070a4761-d1a7-4d3a-811e-f52c3a7d5013" />

## Structure du projet

```
CAN-website/
├── html/                       # Pages du site
│   ├── accueil.html
│   ├── cartes_embarquement.html
│   ├── facture.html
│   ├── statistiques.html
│   └── tableau_bord.html
├── js/                         # Un script par page
│   ├── jscarte.js              # Cartes d'embarquement
│   ├── jsfact.js               # Calcul de la facture
│   ├── jsstat.js               # Statistiques
│   └── jstabbord.js            # Tableau de bord
├── css/style1.css              # Styles globaux
├── img/                        # Logos, icônes, fonds
├── video/                      # Vidéo de présentation
└── download/CAN-software.zip   # Application CAN (projet complémentaire)
```

## Utilisation

### Étapes
1. Cloner le dépôt :
```bash
git clone https://github.com/EmileF67/CAN-website.git
```
2. Ouvrir le fichier `html/accueil.html` dans un navigateur.
