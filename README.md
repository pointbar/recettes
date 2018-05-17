# Recettes

Afficher des recettes de cuisine en utilisant des contenus en markdown et un générateur de site jekyll pour la mise en page

{{ site.description }}

Permet d'afficher les recettes et de naviguer par auteur ou catégories

## Liste d'idées

Le suivi des fonctionnalité est organisé sur la [section *project*](https://github.com/akakeronos/recettes/projects/1) du dépôt d'origine.

## Environnement de développement

Le site utilise un thème en remote *_config.yml* :

```yaml
remote_theme: pointbar/minima
```

Un type de layout "pages" a été défini pour permettre l'affichage des recettes

À cause de cela, pour servir le projet en local il faut installer une dépendance *gem github-pages* dans le *Gemfile*

L'installer :

```bash
bundle install
```

Pour jouer en local, j'utilise *bundle exec* pour contourner les conflits de dépendance :

```bash
bundle exec jekyll serve
```