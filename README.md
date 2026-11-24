# Science des réseaux sociaux et économiques

Site du cours, prêt pour **GitHub Pages** (Jekyll, sans thème externe).

## Mise en ligne

1. Créer un dépôt GitHub et y pousser le contenu de ce dossier.
2. *Settings → Pages → Build and deployment → Deploy from a branch* → branche `main`, dossier `/ (root)`.
3. Le site est publié sur `https://<utilisateur>.github.io/<dépôt>/`.
4. Si le site est dans un sous-chemin (cas général), décommenter et adapter `baseurl` dans `_config.yml`.

## Structure

- `index.md` : page d'introduction.
- `_chapitres/NN-nom.md` : un fichier par chapitre (Markdown). Le champ `ordre` dans l'en-tête fixe l'ordre dans le menu.
- `_layouts/default.html` : mise en page (menu latéral, navigation précédent/suivant).
- `assets/style.css` : styles (thème clair/sombre automatique).

## Ajouter un chapitre

Copier un fichier de `_chapitres/`, changer `title` et `ordre`. Le menu et la navigation se mettent à jour tout seuls.
Les formules LaTeX sont supportées avec `$...$` (MathJax).

## Aperçu local (optionnel)

    gem install bundler jekyll
    jekyll serve
