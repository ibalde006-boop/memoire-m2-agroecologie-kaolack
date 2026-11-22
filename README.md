# Agroécologie et diversité alimentaire des ménages à Kaolack (Sénégal)

Code d'analyse du mémoire de Master 2 en Agroécologie et Systèmes Alimentaires Durables (ASAD),
Université du Sine Saloum El Hadj Ibrahima Niass (USSEIN), Kaolack.

**Auteur :** Ibrahima Baldé
**Encadrant :** Dr Pape Ngore Sadio

## Objectif

Étudier le lien entre l'adoption de pratiques agroécologiques et la diversité alimentaire des ménages
agricoles urbains et périurbains de la commune de Kaolack (enquête de terrain, 178 ménages : 89 urbains
et 89 périurbains).

Deux indicateurs principaux :
- **IAA** : Indice d'Adoption Agroécologique, somme de 25 pratiques notées de 0 à 3 (score brut sur 75) ;
- **HDDS / WDDS** : scores de diversité alimentaire du ménage et des femmes en âge de procréer.

## Contenu

| Notebook | Chapitre du mémoire | Ce qu'il fait |
|---|---|---|
| `notebooks/Analyse_Chapitre_6.ipynb` | Chapitre 6 | Profil des ménages, foncier, validation de l'IAA, typologie (ACP + CAH), diversité alimentaire |
| `notebooks/Analyse_Chapitre_7.ipynb` | Chapitre 7 | Régressions de Poisson, médiation (modèle 4 de Hayes), modération |

Les tableaux et figures produits sont écrits dans un dossier `outputs/`, créé automatiquement.

## Utilisation

1. Installer les bibliothèques : `pip install -r requirements.txt`
2. Placer la base d'enquête `Base_Enquete_Kaolack_178.xlsx` dans un dossier `data/`
3. Lancer `jupyter lab` depuis la racine du dépôt
4. Ouvrir les notebooks et exécuter les cellules dans l'ordre

## Données

La base brute contient des informations sur des ménages et n'est **pas publiée**.
Elle peut être communiquée sur demande, après accord de l'auteur et de l'encadrant.

## Méthodes

- Comparaisons urbain / périurbain : t de Student ou Mann-Whitney, khi-deux ou test exact de Fisher
- Régressions de comptage : Poisson avec erreurs robustes HC3, binomiale négative en comparaison
- Médiation : modèle 4 de Hayes, bootstrap (5 000 réplications)
- Python : pandas, statsmodels, pingouin, scikit-learn, scipy

## Comment citer

Baldé, I. (2026). Agroécologie et diversité alimentaire des ménages à Kaolack : code d'analyse du mémoire de Master 2 ASAD [Code source]. GitHub. https://github.com/ibalde006-boop/memoire-m2-agroecologie-kaolack
