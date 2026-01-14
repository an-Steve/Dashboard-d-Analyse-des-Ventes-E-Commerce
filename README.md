## Dashboard d'Analyse des Ventes E-Commerce
# Réalisé par ANTON NELCON Steve

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7%2B-red)
![License](https://img.shields.io/badge/License-MIT-green)

Un dashboard interactif complet pour l'analyse de données de ventes e-commerce

<img width="1273" height="687" alt="image" src="https://github.com/user-attachments/assets/a3e44ded-09f1-4793-8afc-3a9dc25a2c05" />
<img width="1295" height="656" alt="image" src="https://github.com/user-attachments/assets/0d1f9e41-de90-4152-a2ad-f08d8d5bb392" />
<img width="1290" height="646" alt="image" src="https://github.com/user-attachments/assets/abd74c74-1831-40e2-a6b4-09b9b599d9eb" />
<img width="1291" height="656" alt="image" src="https://github.com/user-attachments/assets/e6a078cb-7b85-431d-8e8a-e566e40a1a18" />
<img width="1291" height="697" alt="image" src="https://github.com/user-attachments/assets/b738d372-a812-478e-9396-50b446526d65" />


#  Fonctionnalités
# Analyse de Données

    Génération de données de vente réalistes (500 transactions)

    Calcul des KPI principaux :

        Chiffre d'affaires total

        Nombre de transactions

        Panier moyen

        CA moyen par vente

    Classement des produits et régions

    Évolution mensuelle des ventes

# Visualisations Graphiques

    4 graphiques principaux :

        Barres : CA par produit

        Camembert : Répartition par région

        Ligne : Évolution mensuelle

        Histogramme : Distribution des prix

    Heatmap : CA par produit et région

    Style moderne avec thème "seaborn-darkgrid"

# Interface Web Interactive

    Dashboard HTML/CSS moderne

    Design responsive

    Cartes de statistiques avec animations

    Tableaux triables

    Badges et indicateurs visuels

    Alertes informatives

Un dashboard interactif complet pour l'analyse de données de ventes e-commerce, entièrement contenu dans un seul fichier Python.


##  Installation Rapide

### Prérequis
```bash
Python 3.8 ou supérieur
pip installé
```

### Installation en 1 minute
```bash
# Téléchargez le fichier
# Ou exécutez directement :
python dashboard_ventes.py
```

### Installation des dépendances (si nécessaire)
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

##  Utilisation

### Mode Jupyter Notebook (Recommandé)
```python
# Copiez-collez tout le code dans une cellule Jupyter
# Exécutez la cellule
# Le dashboard s'affichera automatiquement
```

### Mode Script Python
```python
# Sauvegardez le code dans un fichier .py
python dashboard_ventes.py

# Pour sauvegarder l'HTML :
with open('dashboard.html', 'w', encoding='utf-8') as f:
    f.write(html_content)
```

##  Structure du Code

### 1. **Configuration et Import**
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
# ... autres imports
```

### 2. **Génération des Données**
- 500 transactions e-commerce
- 5 catégories de produits
- 4 régions géographiques
- Données temporelles sur 1 an

### 3. **Nettoyage des Données**
- Gestion des valeurs manquantes
- Suppression des doublons
- Calcul des métriques

### 4. **Analyse Statistique**
```python
ca_total = df['CA'].sum()
top_produits = df.groupby('Produit')['CA'].sum()
ventes_mensuelles = df.groupby('Mois')['CA'].sum()
```

### 5. **Interface HTML/CSS**
- Design moderne avec gradient
- Grid layout responsive
- Animations CSS3
- Couleurs cohérentes

### 6. **Visualisations Matplotlib**
- Subplots organisés
- Style cohérent
- Labels et titres en français

##  Métriques Calculées

| Métrique | Description | Formule |
|----------|-------------|---------|
| **CA Total** | Somme des chiffres d'affaires | `∑(Prix × Quantité)` |
| **Transactions** | Nombre total de ventes | `count(transactions)` |
| **Panier Moyen** | CA moyen par transaction | `CA Total / Transactions` |
| **CA Moyen** | CA moyen par ligne de vente | `mean(CA)` |
| **Top Produits** | Classement des meilleurs vendeurs | `groupby('Produit')['CA'].sum()` |
| **Performance Région** | Répartition géographique | `groupby('Region')['CA'].sum()` |

##  Personnalisation

### Modifier les données
```python
# Changer le nombre de transactions
n_ventes = 1000  # Au lieu de 500

# Ajouter de nouveaux produits
produits = ['Laptop', 'Smartphone', 'Tablette', 'Écouteurs', 'Montre', 'Clavier', 'Souris']
```

### Changer le style
```python
# Modifier la palette de couleurs
sns.set_palette("rocket")  # Au lieu de "husl"

# Changer le thème Matplotlib
plt.style.use('ggplot')  # Au lieu de 'seaborn-darkgrid'
```

### Ajouter de nouvelles régions
```python
regions = ['Nord', 'Sud', 'Est', 'Ouest', 'Centre', 'Île-de-France']
```

## 📱 Compatibilité

- **Environnements supportés** :
  - Jupyter Notebook
  - JupyterLab
  - Google Colab
  - Script Python standalone
  - VS Code avec extension Python

- **Navigateurs** :
  - Chrome (recommandé)
  - Firefox
  - Safari
  - Edge

## 🚨 Résolution de Problèmes

### Problème : Erreur d'import
```bash
# Si pandas n'est pas installé :
pip install pandas numpy matplotlib seaborn
```

### Problème : Graphiques non affichés
```python
# Ajouter en début de script :
import matplotlib
matplotlib.use('TkAgg')  # Ou 'Qt5Agg' selon votre OS
```

### Problème : CSS non appliqué
- Vérifier que vous êtes en environnement Jupyter
- Exécuter toutes les cellules dans l'ordre
- Recharger la page si nécessaire

## 📈 Exemples de Sortie

### 1. **Dashboard HTML**
![Dashboard Preview](https://via.placeholder.com/800x400/667eea/ffffff?text=Dashboard+Interactif)

### 2. **Graphiques**
- Visualisations professionnelles
- Couleurs cohérentes
- Légendes claires
- Axes bien labellisés

### 3. **Tableaux**
- Données en rouge pour visibilité
- Tri possible
- Design responsive

## 🔧 Technologies Utilisées

| Technologie | Version | Usage |
|-------------|---------|-------|
| **Python** | 3.8+ | Langage principal |
| **Pandas** | 2.0+ | Manipulation données |
| **NumPy** | 1.24+ | Calculs numériques |
| **Matplotlib** | 3.7+ | Visualisations |
| **Seaborn** | 0.12+ | Styles avancés |
| **HTML/CSS** | 5/3 | Interface web |
| **Jupyter** | 1.0+ | Environnement interactif |

## 📝 Licence

Ce projet est sous licence MIT. Vous êtes libre de :
- Utiliser le code commercialement
- Modifier et adapter
- Distribuer
- Utiliser en privé

## 👨‍💻 Auteur

**ANTON NELCON Steve**
- Développeur Python/Data Science
- Spécialisé en visualisation de données
- Création de dashboards interactifs

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. Fork le projet
2. Créez une branche (`git checkout -b feature/AmazingFeature`)
3. Committez vos changements (`git commit -m 'Add AmazingFeature'`)
4. Push sur la branche (`git push origin feature/AmazingFeature`)
5. Ouvrez une Pull Request

## 📞 Support

Pour toute question ou problème :
1. Vérifiez la section "Résolution de problèmes"
2. Ouvrez une issue sur GitHub
3. Contactez l'auteur via le profil GitHub

## 🎯 Cas d'Utilisation

### Pour les entreprises :
- Analyse rapide des ventes
- Tableau de bord pour réunions
- Détection de tendances
- Aide à la décision

### Pour les étudiants :
- Apprentissage Python/DataViz
- Exemple complet de projet
- Base pour projets personnels

### Pour les développeurs :
- Template de dashboard
- Code réutilisable
- Architecture modulaire

---

** Conseil Pro** : Pour une analyse plus approfondie, ajoutez :
- Prévisions avec SARIMA
- Analyse RFM (Récence, Fréquence, Montant)
- Segmentation clients
- Analyse de cohortes

---
*Dernière mise à jour : Janvier  2026*
