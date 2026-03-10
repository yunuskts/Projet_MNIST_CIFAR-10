# Classification d'images — Réseaux de neurones & CNN 🧠

Dense + CNN sur MNIST et CIFAR-10 — Accuracy : **97.73%**

## Description
Implémentation et comparaison de réseaux de neurones fully-connected
et convolutifs (CNN) pour la classification d'images.
Étude de l'impact des hyperparamètres et de la taille du dataset.

## Approche

### MNIST — Réseau Dense
- Baseline sans couche cachée : 92.25%
- Impact du nombre de couches et neurones
- Régularisation par Dropout
- Comparaison optimizers : SGD vs Adam
- Normalisation pixels /255, one-hot encoding des labels

### CIFAR-10 — CNN
- Architecture : Conv2D → MaxPooling → Dense
- Implémentation LeNet
- Courbe performance vs taille du dataset (300 → 5900 images)
- Relation logarithmique data/performance
- Analyse des courbes d'entraînement et détection overfitting

## Résultats
| Modèle | Dataset | Accuracy |
|--------|---------|----------|
| Dense baseline (0 couche cachée) | MNIST | 92.25% |
| Dense + 2 couches + Dropout | MNIST | **97.73%** |
| CNN simple | CIFAR-10 | ~60% |

## Leçon clé
Les CNN nécessitent beaucoup de données pour surpasser
les méthodes classiques — lien direct avec l'histoire
de l'IA (stagnation 1990–2012, révolution AlexNet 2012).

## Stack
Python · TensorFlow · Keras · CNN · Conv2D · MaxPooling
· Dropout · Adam · SGD · MNIST · CIFAR-10
