---
title: Navigation autonome de guides et cathéters en cardiologie interventionnelle
date: '2019-02-01'
summary: 'Thèse CIFRE Inria – Robocath : simulation par éléments finis, planification et commande, validation sur robot physique et fantôme.'
tags:
- SOFA
- MCTS
- Cardiologie interventionnelle
- Thèse
---

Navigation robotisée automatique de guides et de cathéters dans les artères coronaires, en trois parties :

1. **Simulation** : modélisation dynamique par éléments finis (SOFA) des artères et de leur interaction avec les instruments chirurgicaux.
2. **Commande** : programmation quadratique (modèle inverse), apprentissage par renforcement et recherche arborescente de Monte Carlo (MCTS) pour la planification.
3. **De la simulation à la réalité** : boucle de planification en simulation, exécution sur le robot physique, recalage de la simulation ; validation sur robot et fantôme, avec des algorithmes de vision par ordinateur pour détecter le guide.

![Simulation de navigation dans l'arbre coronaire](featured.png)

![Maillage d'artères coronaires](maillage-coronaires.png)

![Planification de la navigation](planification.png)

![Boucle de la simulation vers le robot réel](schema-sim-reel.png)

Les apports théoriques et algorithmiques sont publiés dans [RoboSoft 2022](/publications/schegg-2022-robosoft/) et le brevet [WO2023280641](/publications/brevet-wo2023280641/). Les validations sur robot physique et fantôme ne sont publiées que dans le [manuscrit de thèse](/publications/schegg-2022-these/) (sous embargo). Encadrement : C. Duriez, J. Dequidt, P. Preux, B. Fournier.
