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
# 📊 Interprétation des Résultats du Modèle

## ✔️ Coefficient de détermination (R²) = **94%**
Un R² de 94% signifie que **94 % de la variance des ventes est expliquée par le modèle**.  
En d'autres termes, le modèle capture très bien la relation entre les budgets publicitaires (TV, Radio, Newspaper) et les ventes.  
Un R² aussi élevé indique une excellente capacité prédictive dans ce contexte.

---

## ✔️ RMSE = **1.35**
Le RMSE (Root Mean Squared Error) représente l’erreur moyenne entre les valeurs prédites et les valeurs réelles.  
Un RMSE de **1.35** signifie que, **en moyenne, les prédictions du modèle s'écartent de 1,35 unité de vente** par rapport aux valeurs observées.  

➡️ Plus le RMSE est faible, plus les prédictions sont proches de la réalité.  
➡️ Dans ce projet, un RMSE de 1.35 est considéré comme **faible**, ce qui confirme que le modèle est performant.

---

## 📌 Conclusion
Ces deux métriques montrent que le modèle de **régression polynomiale multivariée** prédit efficacement les ventes à partir des budgets publicitaires et capture correctement les relations présentes dans les données.


---

# 📦 Technologies Utilisées
- Python 3.x  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib / Seaborn  

