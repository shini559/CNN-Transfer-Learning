# Détection de Pneumonie par Transfert Learning (DenseNet121 vs MobileNetV2)

Ce projet a pour but de détecter la pneumonie à partir de radiographies pulmonaires en utilisant des techniques de transfert learning avec les modèles pré-entraînés DenseNet121 et MobileNetV2. Il intègre également MLflow pour suivre les expériences, les métriques et les modèles.

## 📁 Architecture du projet

```
CNN_Transfer_Learning/
│
├── data/
│   └── chest_xray/
│       ├── train/
│       │   ├── NORMAL/
│       │   └── PNEUMONIA/
│       ├── val/
│       │   ├── NORMAL/
│       │   └── PNEUMONIA/
│       └── test/
│           ├── NORMAL/
│           └── PNEUMONIA/
│ 
├── models/
│   └── final_model_densenet.h5        # Modèle DenseNet121 entraîné
│
├── CNN_Transfer_Learning.ipynb    # Notebook principal
├── requirements.txt               # Fichier de dépendances
└── README.md
```

## 🚀 Lancer le projet


### 1. Installer les dépendances

```bash
pip install -r requirements.txt
```

### 2. Lancer MLflow en local

```bash
mlflow ui
```

Accéder à l'interface : [http://localhost:5000](http://localhost:5000)

## ✅ Fonctionnalités principales

- Chargement et augmentation des données
- Classification binaire : Pneumonia vs Normal
- Entraînement avec transfert learning (DenseNet121)
- Suivi des expériences avec MLflow (métriques, modèles, paramètres)
- Visualisation des performances via des matrices de confusion et courbes

## 🤝 Contribution

Tu peux contribuer en :

- Proposant des améliorations du code
- Ajoutant d'autres architectures de modèles
- Améliorant l’évaluation ou les visualisations

## 📄 Licence

Ce projet est sous licence **MIT**. Tu peux l'utiliser librement à des fins personnelles ou professionnelles.
