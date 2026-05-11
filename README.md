# Obesity Classification

Projet de classification supervisée pour prédire le statut pondéral d'un individu (Underweight, Normal, Overweight, Obesity) à partir de données médicales. Le pipeline inclut l'exploration des données, l'entraînement de plusieurs classifieurs, la robustesse au bruit, la réduction de dimension.


## Données

- **Source** : https://www.kaggle.com/datasets/suleymansulak/obesity-dataset`
- **Classes** : `Underweight`, `Normal`, `Overweight`, `Obesity`


##  Modèles entraînés

Le projet s'appuie sur une Régression Logistique (OvR) avec une implémentation personnalisée, ainsi que sur le modèle Naïve Bayes Gaussien. Pour la classification basée sur le voisinage et les structures arborescentes, on retrouve le K-Nearest Neighbors (KNN), le Decision Tree, et le modèle d'ensemble AdaBoost. Enfin, plusieurs variantes de machines à vecteurs de support ont été testées, à savoir le SVM Linéaire, le SVM Soft Margin et le SVM RBF.


## Meilleur modèle

Suite aux phases de test et de comparaison, le modèle **AdaBoost** s'est imposé comme le plus performant. En utilisant un **Arbre de Décision** comme estimateur de base, AdaBoost a permis de "booster" ses performances en corrigeant successivement les erreurs des modèles faibles. 


## SetUp

```bash
git clone https://github.com/cestbryan-ng/Obesity-Classification.git
cd Obesity-Classification

pip install -r requirements.txt
```
