# Classification d'un patient en fonction de la présence, ou non, d'une pathologie cardiaque 

Le but de ce projet est de prévoir si un patient a une pathologique cardiaque ou non. La question à laquelle il est nécessaire répondre était la suivante :
> Avec le dossier médical d'un patient, pouvons-nous prédire s'il a un dysfonctionnement cardiaque ou non ?

## Résumé de la démarche
La réalisation du projet a été faite dans Jupyter Notebook grâce au langage Python. Tout d'abord, une analyse de données exploratoire (EDA) a été faite grâce aux packages Matplotlib, Pandas, Numpy et Seaborn. Celle-ci a permit d'observer que la proportion entre patients malades et patients sains est assez homogène ; a également été mis en avant que le genre semble être une variable importante. 

La base de données ne contenait aucune valeur NaN et elle comportait que des variables au format numérique (int 64). Aucun formatage ou normalisation des données n'a donc eu besoin d'être effectué.

La création du modèle de classification des patients a été mis en place. Tout d'abord, la base de données a été divisée en deux échantillons : celui d'entraînement et celui de test. 

Trois modèles ont été testés afin de savoir lequel était le plus performant. Les modèles étaient, "LogisticRegression", "KNeighborsClassifier", "RandomForestCLassifier". Après l'utilisation d'hyperparamétrage afin de rendre les modèles plus précis, le plus performant était "LogisticRegression" ; c'est donc ce dernier qui a été utilisé pour la classification des patients. Enfin, une prédiction a eu lieu sur l'échantillon de validation. L'utilisation de plusieurs métriques a été faite pour mesurer la performance du modèle. 

## Résultats
![download](https://github.com/user-attachments/assets/95d927d4-c268-48a0-9489-d6c8feda681d)

* Accuracy = 0.85
* Précision = 0.82
* Recall = 0.92
* F1-score = 0.87   
