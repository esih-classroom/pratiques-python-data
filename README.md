# Python Data L4 : les pratiques en classe

Un notebook par séance, avec tout ce qu'on écrit ensemble en classe. Consultez-le sur GitHub quand vous voulez, ou clonez le dépôt pour le relancer chez vous.

| Séance | Notebook | Thème |
|---|---|---|
| 0 | `seance-00-prise-en-main.ipynb` | uv, VS Code et les notebooks |
| 1 | `seance-01-premiers-tableaux.ipynb` | NumPy, Series, DataFrame, lire un CSV |
| 2 | `seance-02-selectionner.ipynb` | `loc`, `iloc`, filtres, tri, colonnes calculées |
| 3 | `seance-03-nettoyer.ipynb` | valeurs manquantes, types, doublons, texte, dates |
| 4 | `seance-04-regrouper.ipynb` | `groupby`, `agg`, `value_counts`, `pivot_table` |
| 5 | `seance-05-combiner.ipynb` | `merge`, `concat`, fichiers Excel |
| 6 | `seance-06-visualiser.ipynb` | matplotlib et `df.plot` |
| 7 | `seance-07-statistiques.ipynb` | statistiques descriptives, corrélation |
| 8 | `seance-08-machine-learning.ipynb` | scikit-learn : régression, classification, évaluation |

## Les données

Le fil rouge du cours : les prix des produits de base (riz, maïs, haricot, huile...) dans les marchés des 10 départements, de janvier 2024 à décembre 2025. Les données sont fictives mais réalistes.

| Fichier | Contenu |
|---|---|
| `donnees/prix_marches.csv` | 2 304 relevés propres : mois, département, marché, produit, unité, prix en gourdes |
| `donnees/prix_marches_brut.csv` | les mêmes relevés tels qu'ils arrivent du terrain : valeurs manquantes, doublons, fautes de saisie (séance 3) |
| `donnees/departements.csv` | chef-lieu, population (estimation IHSI 2015) et superficie des 10 départements (séance 5) |
| `donnees/produits.csv` | catégorie, unité et origine (importé ou local) de chaque produit (séance 5) |

## Relancer un notebook chez vous

```bash
cd cours-python
gh repo clone esih-classroom/pratiques-python-data
cd pratiques-python-data
uv sync
code .
```

Dans VS Code, ouvrez le notebook, choisissez le noyau `.venv` en haut à droite, puis **Run All**.
