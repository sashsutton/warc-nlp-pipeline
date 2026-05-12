# Projet Marsactu

Analyse diachronique du corpus web archivé de **Marsactu** (média de presse en ligne marseillais, archivé par la BnF), dans le cadre d'un stage interdisciplinaire histoire / informatique.

- **Auteur :** Sasha Sutton
- **Encadrement :** Sophie Gebeil & Line Jamet-Jakubiec
- **Python :** 3.11

## Structure du dépôt

```
projet-marsactu/
├── README.md
├── requirements.txt
├── data/
│   ├── raw/         # WARC bruts (non versionnés)
│   ├── processed/   # textes extraits
│   └── outputs/     # résultats d'analyses
├── notebooks/       # exploration et analyses
├── src/             # modules réutilisables
├── tests/
└── reports/         # figures et rapports produits par les analyses
```

## Mise en route

Projet développé avec **Python 3.11** (via conda) :

```bash
conda create -n marsactu python=3.11
conda activate marsactu
pip install -r requirements.txt
jupyter notebook
```

## Plan — première partie

### Phase 0 — Mise en place
- Dépôt Git, environnement virtuel, structure de dossiers
- `requirements.txt` minimal (pandas, jupyter, warcio, trafilatura)

### Phase 1 — État de l'art
- Lectures : Milligan, Brügger, Gebeil
- Recensement des outils (SolR Wayback, warcio, trafilatura)
- Synthèse rédigée à part

### Phase 2 — Préparation du corpus
- Installation et indexation SolR Wayback (échantillon)
- Pipeline d'extraction WARC -> DataFrame `pandas`
- Nettoyage, dédoublonnage
- Frise de la volumétrie temporelle
