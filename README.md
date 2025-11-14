# Modèle de Prédiction des Ventes – Régression Polynomiale Multivariée
### *Projet de prédiction des ventes basé sur le dataset Advertising*

---

# 🎯 Objectif du Projet
L’objectif de ce projet est de **prédire les ventes** d’un produit en fonction des investissements publicitaires réalisés sur trois canaux : **TV**, **Radio** et **Newspaper**.  
Pour capturer les relations potentiellement **non linéaires**, une **régression polynomiale multivariée** a été utilisée.

---

# 🗂️ Dataset : Advertising
Le dataset Advertising contient **200 échantillons** avec les variables suivantes :

- **TV** : Budget publicitaire TV (en milliers de dollars)  
- **Radio** : Budget publicitaire Radio  
- **Newspaper** : Budget publicitaire Presse écrite  
- **Sales** : Ventes du produit (variable cible)

---

# 🛠️ Techniques Utilisées

## 🔹 Prétraitement des Données
- Vérification du dataset (aucune valeur manquante).  
- Normalisation des données pour améliorer la stabilité du modèle.  
- Analyse exploratoire et visualisation des relations entre variables.

## 🔹 Découpage du Dataset (Data Split)
- **80%** pour l’entraînement  
- **20%** pour le test  
- Assure une évaluation fiable de la performance du modèle.

## 🔹 Modélisation : Régression Polynomiale Multivariée
- Génération de features polynomiales (`PolynomialFeatures`).  
- Entraînement d’un modèle de régression linéaire sur ces nouvelles features.  
- Optimisation du degré du polynôme selon les métriques (**MSE**, **RMSE**, **R²**).

---

# 📊 Évaluation du Modèle
- Analyse des performances sur les données de test.  
- Visualisation des prédictions vs valeurs réelles.  
- Interprétation de l’impact des budgets publicitaires sur les ventes.

---

# 📦 Technologies Utilisées
- Python 3.x  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib / Seaborn  

---

# 🚀 Résultats et Valeur Ajoutée
- Pipeline complet : **prétraitement → modélisation → évaluation**.  
- Identification des canaux publicitaires ayant le plus d’impact (TV et Radio).  
- Base solide pour tester d'autres modèles (Ridge, Lasso, Random Forest…).

---

# 📁 Structure du Projet
