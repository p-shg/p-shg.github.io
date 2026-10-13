# Site personnel de Pierre Schegg (Hugo Blox, modèle `academic-cv`)

Site statique en français : accueil (bio, recherche), publications (articles, communications, thèse, brevets),
projets, enseignement et encadrement, parcours (expérience, compétences, service).

## Publier sur GitHub Pages

1. Créer un dépôt GitHub (par exemple `pierreschegg.github.io`) et y pousser ce dossier sur la branche `main`.
2. Dans *Settings → Pages*, choisir **GitHub Actions** comme source. Le workflow `.github/workflows/deploy.yml`
   compile (`hugo --minify`) et publie à chaque `git push`.
3. Domaine personnalisé (optionnel) : ajouter le domaine dans *Settings → Pages* et un enregistrement DNS.

## En local

```bash
# Hugo extended >= 0.162 (cf. hugoblox.yaml), Go et Node
pnpm install
hugo server        # http://localhost:1313
```

## Où modifier quoi

| Élément | Fichier |
|---|---|
| Identité, bio, liens, formation, expérience, compétences | `data/authors/me.yaml` |
| Page d'accueil | `content/_index.md` |
| Publications, communications, thèse, brevets | `content/publications/<slug>/index.md` |
| Projets | `content/projects/<slug>/index.md` |
| Enseignement et encadrement | `content/teaching.md` |
| Parcours, service, collaborations | `content/experience.md` |
| Menu | `config/_default/menus.yaml` |
| Nom du site, description, thème, licence | `config/_default/params.yaml` |
| Photo de profil | `assets/media/authors/me.jpg` (à ajouter) |

Voir `A_COMPLETER.md` pour la liste de ce qui manque ou reste à vérifier.
