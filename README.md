🎨 Fine-Tuning de ResNet18 sur le Dataset MNIST

Ce projet présente une implémentation complète du fine-tuning du modèle ResNet18 sur le dataset MNIST, un classique de la classification d’images manuscrites.
L’objectif est d’adapter un modèle pré-entraîné sur ImageNet à une tâche plus simple : la classification de chiffres (0–9).

🚀 Objectifs du projet

Charger et préparer le dataset MNIST pour un réseau convolutif pré-entraîné.

Adapter ResNet18 pour une nouvelle tâche de classification.

Entraîner, optimiser et évaluer les performances du modèle.

Visualiser les métriques d'entraînement : perte, précision, etc.

🧠 Architecture utilisée
🔹 ResNet18 (pré-entraîné sur ImageNet)

Résidus d'identité et convolutionnels.

Très efficace même sur de petits datasets.

Dernière couche modifiée pour 10 classes (sortie MNIST).

🔧 Technologies utilisées

Python

PyTorch

Torchvision

Matplotlib

Jupyter Notebook

📂 Structure du projet
📁 FineTuning-ResNet18-MNIST
│
├── FINE_TUNING_RESNET18_SUR_MNIST.ipynb
└── README.md

🛠️ Préparation des données

Conversion MNIST en format 3 canaux (RGB) pour correspondre à ImageNet.

Normalisation avec les statistiques standards ImageNet.

Split train / test.

Utilisation de DataLoader pour batching efficace.

🏋️ Entraînement

Optimiseur : Adam ou SGD

Loss : CrossEntropyLoss

Scheduler (optionnel)

Fine-tuning total ou partiel selon les couches gelées

📊 Évaluation

Calcul de la précision sur le dataset test

Visualisation :

courbe de perte (loss)

évolution de la précision

matrice de confusion (si incluse dans ton notebook)
