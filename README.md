# Prédiction des frais médicaux - Modélisation avec Scikit-Learn

## 📌 Objectif du projet

Ce projet vise à prédire les **frais médicaux (`charges`)** facturés à des individus à partir de caractéristiques telles que l'âge, le sexe, le statut de fumeur, l'IMC, le nombre d'enfants et la région. L'analyse repose sur le jeu de données classique `insurance.csv`.

## 🧰 Technologies utilisées

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- seaborn

## 📂 Contenu du projet

- `insurance.csv` : Jeu de données contenant les informations des patients.
- `main.ipynb` :
  - L’analyse exploratoire des données (EDA)
  - L'encodage des variables catégorielles
  - La normalisation optionnelle
  - Les modèles de régression :
    - Régression linéaire
    - Arbre de décision
    - XGBoost Regressor
  - L’évaluation des performances (MSE, RMSE, R²)
  - Les visualisations (prédictions vs valeurs réelles)

## 🧪 Modèles testés

- **Régression linéaire**
- **DecisionTreeRegressor**
- **XGBRegressor**

## 📊 Métriques d'évaluation

Les performances des modèles sont mesurées à l’aide de :

- `MSE` : Mean Squared Error
- `RMSE` : Root Mean Squared Error
- `R²` : Coefficient de détermination

## 📈 Exemple de visualisation

Un graphique `scatter` est généré pour comparer les **valeurs prédites** aux **valeurs réelles** des charges.

## 🔄 Prétraitement

- Transformation des variables catégorielles via `pd.get_dummies()`
- Option : transformation logarithmique de `charges` via `np.log(charges)` pour améliorer la linéarité.
