---
title: ''
summary: ''
date: '2026-10-13'
type: landing
sections:
- block: resume-biography-3
  content:
    username: me
    text: ''
    headings:
      about: ''
      education: ''
      interests: ''
  design:
    background:
      gradient_mesh:
        enable: true
    name:
      size: md
    avatar:
      size: medium
      shape: circle
- block: markdown
  content:
    title: Recherche
    subtitle: ''
    text: 'Mes recherches s''articulent autour de deux axes :


      - **Robotique médicale et chirurgicale** : étude du geste chirurgical pour développer des dispositifs médicaux robotiques (chirurgie de l''oreille, cardiologie interventionnelle, chirurgie endoscopique de l''estomac).

      - **Biomécanique** : étude du mouvement humain et de ses déficiences (hémiplégie, paralysies) pour concevoir des solutions robotiques d''assistance et de réadaptation.


      Je suis convaincu que la modélisation et la simulation du corps humain et de ses dysfonctionnements permettent de trouver des solutions technologiques pour améliorer la santé des patients et la qualité de vie des personnes en situation de handicap.


      **Ma démarche : modéliser et simuler → concevoir et fabriquer → contrôler et interagir → valider.**


      **Projet à l''IUT et dans l''équipe DEXTER**


      - *Robotique déformable d''assistance* : comment assister les gestes du quotidien avec des robots déformables ? Conception et fabrication, co-conception robot et modèle musculo-squelettique, commande pour l''interaction humain-robot, interfaces humain-machine, validation clinique.

      - *Robotique endovasculaire* : comment piloter un robot endovasculaire pour une neuroradiologie autonome ? Simulation, commande prédictive, validation préclinique.

      - *Transfert et démonstrateurs* : open source et open hardware, démonstrateurs pour l''enseignement et la communication, projets étudiants.


      Mots-clés : automatique, biomécanique, robotique déformable, robotique médicale, interaction humain-robot, simulation médicale, modélisation par éléments finis (FEM).

      '
  design:
    columns: '1'
- block: collection
  id: papers
  content:
    title: Publications à la une
    filters:
      folders:
      - publications
      featured_only: true
  design:
    view: article-grid
    columns: 2
- block: collection
  content:
    title: Toutes les publications, communications et brevets
    text: ''
    filters:
      folders:
      - publications
      exclude_featured: false
  design:
    view: citation
---
