# Prédiction de la demande en électricité

*Projet disponible ici :* [Notebook](https://github.com/Sylvariane/prediction_conso_electrique/blob/main/P9_01_code.ipynb)

## Détails du projet

Après avoir récupéré les données de la consommation d'électricité et de la température en DJU, il fallait représenter ces deux séries temporelles puis ensuite corriger la consommation d'électricité en fonction de la température par l'intermédiaire d'une régression linéaire. 

![correction](https://user-images.githubusercontent.com/64648386/115601417-185b2d00-a2de-11eb-8ead-eee3f8943132.png)

Une fois ces dispositions prises, il était possible de tester des modèles pour prédire les consommations d'électricité des 12 prochains mois. Deux méthodes ont été utilisés : 
- Le lissage exponentiel de Holt-Winters
- Le modèle SARIMA

**Prédiction avec le modèle de Holt-Winters**
![pred_HW](https://user-images.githubusercontent.com/64648386/115601536-3a54af80-a2de-11eb-8e4b-8eaa69c351fa.png)

**Prédiction avec le modèle SARIMA**
![pred_sarima](https://user-images.githubusercontent.com/64648386/115601616-50fb0680-a2de-11eb-9f88-903c6423ba1a.png)


Le modèle de Holt-Winters est celui qui a obtenu les meilleurs résultats lors de l'évalution du modèle (MAE, MAPE, MSE) par rapport au modèle SARIMA. Cependant, le modèle SARIMA a su capter l'importante baisse mesurée au début de l'anneé 2020.

## Syllabus 

Ce projet a été réalisé dans le cadre de ma formation de Data Analyst.

Les compétences acquises lors de ce projet sont :
- Maîtriser les méthodes de lissage et de Holt-Winters
- Maîtriser les notions de composantes et de modèles de décomposition
- Maîtriser les modèles ARMA
- Représenter graphiquement une série temporelle

Ce projet a été soutenu et validé le 7 janvier 2021.
