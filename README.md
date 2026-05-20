# 👨‍💼 Employees Management System

Un système de gestion des employés développé en **Python**, utilisant **SQLite** pour le stockage des données et **Pandas** pour l’analyse et la manipulation des données.

Ce projet illustre la mise en place d’un système CRUD complet ainsi que l’exploitation des données via des requêtes SQL et des DataFrames.


## 📁 Structure du Projet

```bash
📦 employees-management-system
 ┣ 📄 kompass.ipynb
 ┣ 📄 kompass_employees.db
 ┗ 📄 README.md
```


## 🛠️ Technologies Utilisées

* **Python**
* **SQLite** (base de données légère)
* **Pandas** (analyse de données)
* **Jupyter Notebook**


## 🎯 Objectifs du Projet

Ce projet a été conçu pour :

- ✔️ Implémenter un système de gestion des employés
- ✔️ Manipuler une base de données relationnelle avec SQLite
- ✔️ Appliquer les opérations CRUD (Create, Read, Update, Delete)
- ✔️ Exploiter les données avec Pandas
- ✔️ Écrire et exécuter des requêtes SQL
- ✔️ Analyser des données d’entreprise simples


## 🗄️ Base de Données

Le système utilise une base SQLite :

* **Nom** : `kompass_employees.db`
* **Table principale** : `employees`

### Exemple de champs :

* id
* name
* department
* salary
* (autres attributs selon implémentation)


## ⚙️ Fonctionnalités

### 🔹 Gestion des employés (CRUD)

Le système permet :

* Ajouter un employé
* Afficher la liste des employés
* Mettre à jour les informations
* Supprimer un employé

Ces fonctionnalités sont implémentées dans la classe :

```python
EmployeeManagement
```


### 🔹 Interface Console

Un menu interactif permet de gérer les opérations :

```
1. Ajouter un Employé
2. Afficher les Employés
3. Mettre à Jour un Employé
4. Supprimer un Employé
```


### 🔹 Analyse de Données avec Pandas

Le projet inclut également une partie analytique :

* Lecture des données avec `read_sql_query`
* Transformation en DataFrame
* Analyse des données

#### Exemples :

- ✔️ Afficher tous les employés
- ✔️ Identifier les départements uniques
- ✔️ Calculer des statistiques (ex : moyenne)

```python
df = pd.read_sql_query("SELECT * FROM employees", conn)
```


## 📊 Exemples de Requêtes

* Liste des employés :

```sql
SELECT * FROM employees;
```

* Départements uniques :

```sql
SELECT DISTINCT department FROM employees;
```

* Calcul (ex : moyenne) :

```sql
SELECT AVG(age) FROM employees;
```


## ▶️ Comment Exécuter le Projet

1. Installer les dépendances :

```bash
pip install pandas
```

2. Lancer le notebook :

```bash
jupyter notebook
```

3. Ouvrir :

```
kompass.ipynb
```


## 📈 Workflow du Projet

1. Création de la base SQLite
2. Création de la table `employees`
3. Implémentation de la classe de gestion
4. Interaction via menu console
5. Analyse des données avec Pandas


## 💡 Compétences Démontrées

- ✔️ Manipulation de bases de données SQLite
- ✔️ Programmation orientée objet en Python
- ✔️ Implémentation CRUD
- ✔️ Requêtes SQL
- ✔️ Analyse de données avec Pandas
- ✔️ Structuration d’un mini système de gestion


## 🤝 Contributions

Ce projet est une démonstration pédagogique, mais toute suggestion d’amélioration est la bienvenue.


## 👤 Auteur

**Alex Alkhatib**
Ingénieur en Intelligence Artificielle — Passionné par la Data et le développement Python.


## 📄 Licence

MIT License — Copyright (c) 2026 Alex Alkhatib
