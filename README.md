# Pipeline NLP — Multi-flux RSS

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![spaCy](https://img.shields.io/badge/NLP-spaCy-09A3D5?logo=spacy&logoColor=white)
![NLTK](https://img.shields.io/badge/NLP-NLTK-green)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange?logo=jupyter&logoColor=white)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1wp6RJGc2Fg7XKioOYxi-lphkagmRS1qx)

Pipeline NLP complet pour collecter des flux RSS multi-sources, nettoyer les articles, générer des résumés automatiques et extraire des entités nommées et mots-clés.

---

## Fonctionnalités

| Étape | Description |
|-------|-------------|
| Collecte | Agrégation de flux RSS depuis plusieurs sources |
| Nettoyage | Suppression du HTML, normalisation du texte |
| Résumé | Résumé extractif avec **LexRank** (sumy) |
| Extraction | Entités nommées + mots-clés avec **spaCy** |
| Sortie | Résultats structurés (JSON / affichage console) |

---

## Stack technique

| Composant | Technologie |
|-----------|-------------|
| Collecte RSS | feedparser |
| NLP | spaCy, NLTK |
| Résumé | sumy (LexRank) |
| Notebook | Jupyter / Google Colab |

---

## Fichiers

| Fichier | Description |
|---------|-------------|
| `PDVD_V1ipynb (3).ipynb` | Notebook principal |
| `pdvd_v1ipynb.py` | Script Python équivalent |

---

## Lancer le projet

```bash
pip install feedparser spacy nltk sumy
python -m spacy download fr_core_news_sm
jupyter notebook "PDVD_V1ipynb (3).ipynb"
```

Ou directement sur Google Colab : [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1wp6RJGc2Fg7XKioOYxi-lphkagmRS1qx)

---

## Évolution

Ce projet fait suite à une première version utilisant un format RDF pour structurer les résultats — le pipeline a ensuite évolué vers une approche NLP plus directe avec LexRank.