# Site personnel de Pierre Schegg (Hugo Blox, modèle `academic-cv`)

Site statique en français : accueil (bio, recherche), publications (articles, communications, thèse, brevets),
projets, enseignement et encadrement, parcours (expérience, compétences, service).

## Publier sur GitHub Pages

1. Créer un dépôt GitHub nommé `<utilisateur>.github.io` (ici `p-shg.github.io`) et y pousser ce dossier sur la branche `main`.
2. Dans *Settings → Pages*, choisir **GitHub Actions** comme source. Le workflow `.github/workflows/deploy.yml`
   compile (`hugo --minify`) et publie à chaque `git push`.
3. Domaine personnalisé (optionnel) : ajouter le domaine dans *Settings → Pages* et un enregistrement DNS.

## En local

Prérequis : Go, Node ≥ 22 (`conda create -n site -c conda-forge nodejs=22 && conda activate site`) et Hugo **extended** dans la version de `hugoblox.yaml` (le paquet Ubuntu est trop ancien).

```bash
# Hugo extended 0.162.0 dans ~/.local/bin (à mettre dans le PATH)
wget -qO- https://github.com/gohugoio/hugo/releases/download/v0.162.0/hugo_extended_0.162.0_linux-amd64.tar.gz \
  | tar xz -C ~/.local/bin hugo

npm install          # ou pnpm install
hugo server          # aperçu sur http://localhost:1313
hugo --minify && npx pagefind --site public   # build de production dans public/
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
