Présentation du projet
Ce projet applique des techniques de machine learning pour prédire les pannes d’équipements industriels à partir du dataset AI4I 2020 Predictive Maintenance. L’objectif est de construire un modèle fiable, interprétable et exploitable dans un contexte réel de maintenance.

Objectifs
- Comprendre et analyser un dataset industriel.
- Gérer le déséquilibre des classes avec SMOTE.
- Entraîner un modèle robuste (Random Forest).
- Optimiser le seuil de décision pour maximiser la détection des pannes.
- Interpréter les résultats pour une utilisation opérationnelle.
- Fournir un pipeline clair et reproductible.

Structure du dépôt
- data/ — dataset (ai4i2020.csv).
- notebooks/ — notebook complet du projet (AI4I_predictive_maintenance).
- requirements.txt — dépendances nécessaires.
- .gitignore — fichiers ignorés par Git.
- README.md — documentation du projet.

Modèle final
Le modèle retenu est un Random Forest entraîné sur des données rééquilibrées avec SMOTE.
Un seuil de décision optimisé à 0.3 a été choisi pour maximiser le rappel sur la classe panne.

Résultats principaux
- Accuracy : 0.95
- Recall (panne) : 0.84
- Pannes manquées : 10
- Fausses alertes : 91
Ces performances offrent un compromis adapté à un contexte industriel où il vaut mieux détecter trop que pas assez.

Interprétation du modèle
L’importance des variables montre que le modèle s’appuie sur des facteurs cohérents avec les mécanismes de défaillance :
- Température du process
- Température de l’air
- Vitesse de rotation
- Couple
- Usure de l’outil
Ces variables sont directement liées aux phénomènes physiques observés dans les machines industrielles.

Conclusion
Ce projet propose un pipeline complet de maintenance prédictive, depuis l’analyse des données jusqu’à l’évaluation finale du modèle.
Le modèle obtenu est performant, interprétable et prêt à être utilisé comme base pour une mise en production ou un système de surveillance.

▶️ Installation

pip install -r requirements.txt

