# Analyse de la Performance Commerciale & Segmentation Client
### E-Commerce UK — 2010 / 2011

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python) ![pandas](https://img.shields.io/badge/pandas-2.x-150458?logo=pandas) ![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi)

---

## Contexte

Une entreprise britannique de vente en ligne (cadeaux & décoration) souhaite piloter sa performance commerciale et mieux comprendre la valeur de ses clients.

Ce projet répond à 4 questions métier concrètes :
1. Quelle est l'évolution du CA et de la marge dans le temps ?
2. Quels sont les marchés et produits les plus rentables ?
3. Quel est l'impact financier des retours produits ?
4. Qui sont nos meilleurs clients — et lesquels sont à risque ?

---

## Dashboard Power BI

![Dashboard](https://github.com/ballogou-essi/Ecommerce-performance-analysis/blob/main/D%C3%A9mo/d%C3%A9mo.gif)

Accédez au PDF : [PBX_PDF](https://github.com/ballogou-essi/Ecommerce-performance-analysis/blob/main/PBX/Suivi_retail.pdf)
---

## Structure du projet

```
├── online_retail.csv           # Données brutes (UCI ML Repository)
├── analyse_performance_ecommerce.ipynb  # Notebook principal
├── outputs/
│   ├── fact_transactions.xlsx  # Table de faits — lignes de vente enrichies
│   ├── dim_clients_rfm.xlsx    # Dimension client — scores & segments RFM
│   └── agg_mensuel.xlsx        # Agrégat mensuel — KPIs pour Power BI
└── README.md
```

---

## Étapes du notebook

| # | Étape | Description |
|---|---|---|
| 1 | Audit | Exploration et diagnostic de la donnée brute |
| 2 | Nettoyage | Typage, suppression des anomalies, isolation des retours |
| 3 | Feature Engineering | Variables temporelles, CA, marge estimée, zone géo |
| 4 | Performance commerciale | KPIs, évolution mensuelle, top pays & produits, saisonnalité |
| 5 | Analyse des retours | Impact financier, simulation de scénarios d'amélioration |
| 6 | Segmentation RFM | 5 segments clients : VIP, Fidèles, Occasionnels, À risque, Inactifs |
| 7 | Export | Génération des 3 fichiers d'alimentation Power BI |

---

## Lancer le projet

```bash
pip install pandas numpy matplotlib seaborn openpyxl
jupyter notebook analyse_performance_ecommerce.ipynb
```

> Les 3 fichiers Excel sont générés automatiquement à l'étape 7.

---

## Stack technique

`Python` · `pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Power BI`
