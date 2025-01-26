
# Détection des Maladies des Plantes avec le Dataset PlantVillage

Ce projet porte sur la détection automatique des maladies des plantes en utilisant des techniques d'apprentissage automatique et d'apprentissage profond. Le dataset **PlantVillage** a été utilisé pour entraîner un modèle capable d'identifier différentes maladies des plantes à partir d'images de feuilles.

## Étapes pour créer le modèle

### 1. Préparation des données

- **Dataset** : Le dataset **PlantVillage** contient 54 306 images de feuilles, réparties en 16 classes représentant différentes maladies et feuilles saines.
- **Exploration des données** : Visualisation des images et des classes.
- **Prétraitement** :
  - **Séparation des données** en ensembles d'entraînement, de validation, et de test.
  - **Normalisation** : Les images sont normalisées pour accélérer la convergence du modèle.

### 2. Construction du modèle

- **Type de modèle** : Un **réseau de neurones convolutif (CNN)** a été utilisé pour classifier les images.
- **Architecture** :
  - Couches convolutionnelles pour extraire les caractéristiques visuelles des images.
  - Couches de pooling pour réduire la dimensionnalité.
  - Couches fully connected pour la classification.
  - Softmax à la fin pour prédire les 16 classes.

### 3. Entraînement du modèle

- **Optimiseur** : Utilisation de l'optimiseur **Adam**.
- **Fonction de perte** : **Cross Entropy** pour la classification multi-classes.
- **Taille de batch** : Utilisation d'une taille de batch de 32.
- **Augmentation des données** : Application de techniques d'augmentation des données (rotation, flip) pour améliorer la robustesse du modèle.

### 4. Évaluation du modèle

- **Précision** obtenue : 92%.
- **Courbes de précision et de perte** : Suivi de la performance du modèle durant l'entraînement.
- **Matrice de confusion** : Visualisation des prédictions correctes et incorrectes pour chaque classe.

### 5. Améliorations possibles

- **Augmentation des données** : Appliquer davantage de techniques pour générer plus de diversité dans les données d'entraînement.
- **Optimisation des hyperparamètres** : Ajuster le taux d'apprentissage, la taille du batch, et les époques pour améliorer les performances.
- **Modèles plus complexes** : Essayer des architectures plus avancées comme ResNet pour une meilleure performance.

