Maintenance prédictive – Détection de pannes (AI4I 2020)
Ce projet applique des techniques de machine learning pour prédire les pannes d’équipements industriels à partir du dataset AI4I 2020 Predictive Maintenance Dataset. L’objectif est de construire un modèle performant et exploitable permettant d’anticiper les défaillances avant qu’elles ne surviennent.

Objectifs du projet
• 	Analyser un dataset industriel déséquilibré.
• 	Construire un modèle robuste capable de détecter les pannes.
• 	Gérer le déséquilibre des classes avec SMOTE.
• 	Optimiser le modèle via un seuil de décision personnalisé.
• 	Interpréter les résultats pour une utilisation réelle en maintenance.
• 	Fournir un pipeline clair, reproductible et professionnel.

Contenu du projet
• 	Exploration des données : compréhension des variables, visualisations, nettoyage.
• 	Préparation des données : normalisation, séparation train/test, gestion du déséquilibre.
• 	Modélisation : Random Forest avec SMOTE.
• 	Optimisation : test de plusieurs seuils (0.5 → 0.1) pour maximiser la détection des pannes.
• 	Interprétation : importance des variables.
• 	Évaluation finale : métriques complètes + matrice de confusion.
• 	Conclusion : justification du modèle final.

Modèle final retenu
Le modèle final est un Random Forest entraîné sur des données rééquilibrées avec SMOTE, puis optimisé avec un seuil de décision de 0.3.
Ce seuil offre le meilleur compromis entre :
• 	Recall élevé sur la classe “panne” (0.84)
• 	Faible nombre de pannes manquées (10 sur 2000)
• 	Volume de fausses alertes raisonnable
• 	Stabilité globale du modèle

Résultats principaux
• 	Accuracy : 0.95
• 	Recall (panne) : 0.84
• 	Pannes manquées : 10
• 	Fausses alertes : 91
• 	Importance des variables cohérente avec la physique industrielle (température, vitesse, couple, usure)

Interprétation du modèle
L’importance des variables montre que le modèle s’appuie sur des facteurs pertinents :
• 	Température du process
• 	Température de l’air
• 	Vitesse de rotation
• 	Couple
• 	Usure de l’outil
Ces variables sont directement liées aux mécanismes de défaillance, ce qui renforce la crédibilité du modèle.

Conclusion
Ce projet propose un pipeline complet et professionnel de maintenance prédictive :
• 	Gestion du déséquilibre
• 	Modèle robuste
• 	Optimisation du seuil
• 	Interprétation claire
• 	Résultats exploitables en contexte industriel
Le modèle final est performant, explicable et prêt à être intégré dans un système de surveillance ou utilisé comme base pour une mise en production.

📎 Fichiers inclus
• 	 : notebook complet du projet
• 	 : documentation du projet
• 	 (optionnel) : dépendances Python
