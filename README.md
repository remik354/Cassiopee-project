# GNN Visualisation and Optimization Notebooks

Ce dépôt contient plusieurs notebooks Jupyter pour la visualisation et l'optimisation de modèles de réseaux de neurones graphiques (GNN). Les notebooks couvrent des tâches d'induction et de transduction, ainsi que l'optimisation des hyperparamètres à l'aide d'Optuna.

## Contenu du dépôt

- **Visualisation.ipynb** : Notebook pour visualiser les résultats des modèles GNN.
- **optuna_transduction.ipynb** : Optimisation des hyperparamètres pour les modèles de transduction à l'aide d'Optuna.
- **optuna_induction.ipynb** : Optimisation des hyperparamètres pour les modèles d'induction à l'aide d'Optuna.
- **GATv2_transduction.ipynb** : Implémentation et évaluation du modèle GATv2 pour les tâches de transduction.
- **GATv2_one_graph.ipynb** : Implémentation du modèle GATv2 sur un seul graphe.
- **GATv2_induction.ipynb** : Implémentation et évaluation du modèle GATv2 pour les tâches d'induction.

## Prérequis

Assurez-vous d'avoir les éléments suivants installés avant de commencer :

- Python 3.7 ou supérieur
- Jupyter Notebook
- Bibliothèques Python :
  - numpy
  - pandas
  - matplotlib
  - torch
  - torch-geometric
  - optuna

Vous pouvez installer les bibliothèques nécessaires en exécutant la commande suivante :

```bash
pip install numpy pandas matplotlib torch torch-geometric optuna

Utilisation

Étape 0 : Organiser ses dossiers avec les données

BLCA_DATA/
├── CLINICAL
│ └── PROCESSED
├── HISTO
│ └── PROCESSED
│     ├── DIAGNOSTIC_SLIDES
│     └── TISSUE_SLIDES
├── labels_onehot.csv
├── labels_str.csv
├── node_embedding.csv
├── node_embedding.pt
├── OMICS
│ └── PROCESSED
│     ├── gene-expression_norm.csv
│     ├── methylation_norm.csv
│     ├── mirna-expression_norm.csv
│     └── protein-expression_norm.csv
└── Workspace
    ├── labels_str.csv
    ├── labels_str_Norm_weights.csv
    ├── node_embedding.csv
    └── patient_norm.csv

cassiopee-projet-main/
*travaillez ici*

Organisez vos dossiers selon le modèle suivant : 


Étape 1 : Cloner le dépôt

Clonez le dépôt sur votre machine locale en utilisant la commande suivante :

bash

git clone https://github.com/votre-utilisateur/votre-repo.git
cd votre-repo

Étape 2 : Exécuter les notebooks

Ouvrez Jupyter Notebook et accédez aux différents notebooks pour les exécuter :

bash

jupyter notebook

Étape 3 : Explorer les notebooks

    Visualisation.ipynb : Ce notebook vous permet de visualiser les résultats des différents modèles GNN. Vous pouvez ajuster les paramètres de visualisation selon vos besoins.

    optuna_transduction.ipynb et optuna_induction.ipynb : Utilisez ces notebooks pour optimiser les hyperparamètres des modèles de transduction et d'induction respectivement. Optuna est utilisé pour trouver les meilleures combinaisons d'hyperparamètres.

    GATv2_transduction.ipynb, GATv2_one_graph.ipynb, GATv2_induction.ipynb : Ces notebooks contiennent des implémentations spécifiques du modèle GATv2 pour différentes tâches. Vous pouvez évaluer les performances du modèle et ajuster les paramètres pour améliorer les résultats.