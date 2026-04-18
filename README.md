# Speed Dating — Analyse exploratoire

Analyse du dataset Speed Dating (Tinder) pour comprendre ce qui pousse deux personnes à vouloir se revoir après un premier rendez-vous de 4 minutes.

Projet de certification Jedha — Data Science, bloc #2.

---

## Contexte

Tinder constate une baisse du nombre de matchs. Pour en comprendre les raisons, une expérience de speed dating a été organisée : chaque participant enchaîne des rendez-vous de 4 minutes avec toutes les personnes du sexe opposé et indique secrètement s'il souhaite revoir son partenaire.

L'objectif est d'identifier dans ces données les critères qui déclenchent un "oui", afin de fournir à l'équipe marketing des recommandations actionnables.

## Dataset

- **8 378 rencontres** enregistrées
- **551 participants** (277 hommes, 274 femmes)
- **21 sessions** entre octobre 2002 et avril 2004
- **195 variables** : ratings post-date, préférences déclarées au signup, démographie, décisions

Le fichier `data/tinder_data.csv` contient l'ensemble des données.

## Contenu du repo

```
.
├── data/
│   └── tinder_data.csv
├── tinder.ipynb
└── README.md
```

## Reproduire les analyses

Prérequis : Python 3 avec `pandas`, `numpy`, `plotly` et `statsmodels`.

```bash
pip install pandas numpy plotly statsmodels
```

Ouvrir le notebook :

```bash
jupyter notebook tinder.ipynb
```

Puis "Restart & Run All" pour exécuter toutes les cellules.

## Principaux résultats

- Les **hommes disent "oui" 47 %** du temps, les **femmes 37 %** : deux seuils d'acceptation à traiter séparément.
- Trois attributs font la décision pour les deux genres : **attractivité, fun, intérêts partagés**. Sincérité, intelligence et ambition sont des prérequis, pas des différentiateurs.
- Les participants **surestiment systématiquement** leur propre attractivité (décalage moyen de +0,77 point chez les femmes, +1,02 chez les hommes).
- Les **intérêts partagés** pèsent environ **trois fois plus** que l'origine ethnique dans le taux de match.
- Être le **premier rendez-vous de la soirée** donne un taux de "oui" de 49,9 %, soit 8 points au-dessus de la moyenne.

Détails, graphiques et interprétations complètes dans `tinder.ipynb`.

## Auteur

Ramili Rindra — Jedha Data Science, 2026.
