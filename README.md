# Classification d'un patient en fonction s'il a une maladie du coeur ou non

Le but de ce projet était de prédire si un patient a un maladie du couer ou non. La question à laquelle il fallait répondre était la suivante :
> Avec le dossier médiacal d'un patient, pouvons nous prédire s'il a un dysfonctionnement cardiaque ou non ?

## Résumé de la démarche
La réalisation du projet a été faite dans Jupyter Notebook grâce au language Python. Tout d'abord, une analyse de données exploratoire (EDA) a été faite grâce au packages Matplotlib, Pandas, Numpy et Seaborn. Celle-ci a permit d'observer que la proportion patients malades et non malades était assez équilibrée. Elle a également permit de mettre en avant que le sexe semble être une variable importante. 

Ensuite, la base de données ne contenait aucune valeur NaN et que des variables au format numérique (int 64). Aucun formatage ou normalisation des données n'a donc eu besoin d'être effectué.

Enfin, la création du modèle de classification des patients a été mis en place. D'abord la base de données a été divisée en deux échantillons, celui d'entraînement et celui de test. Trois modèles ont été testés afin de savoir lequel était le plus performant. Les modèles étaient, "LogisticRegression", "KNeighborsClassifier", "RandomForestCLassifier". Après l'utilisation d'hyperparamétrage afin de rendre les modèles plus précis, le plus performant était "LogisticRegression", c'est donc celui-ci qui a été utilisé pour la classification des patients. Enfin, une prédiction a eu lieu sur l'échantillon de validation et l'utilisation de plusieurs métriques on été utilisées pour mésurer la performance du modèle. 

## Résultats
![download](https://github.com/user-attachments/assets/95d927d4-c268-48a0-9489-d6c8feda681d)

* Accuracy = 0.85
* Précision = 0.82
* Recall = 0.92
* F1-score = 0.87   
