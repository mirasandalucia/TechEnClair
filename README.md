# TechEnClair – Ressources Home Assistant

![TechEnClair](images/Logo.webp)

Kit public de snippets YAML, exemples d’automations et espaces prêts à remplir pour vos dashboards, thèmes et assets. Conçu pour démarrer rapidement sans exposer de secrets.

## Contenu du dépôt
```
TechEnClair/
+-- custom-cards/
¦   +-- instructions.md            # prérequis pour certaines cartes custom
+-- dashboards/                    # vos dashboards Lovelace (.yaml)
+-- images/
¦   +-- Logo.webp                  # logo projet
¦   +-- Poubelle.webp              # exemple d’asset
+-- scripts/                       # snippets prêts à copier
¦   +-- automation-examples.yaml
¦   +-- *.txt                      # autres scripts/cartes (ouvrir et copier le YAML)
+-- themes/                        # vos thèmes Home Assistant (.yaml)
+-- .gitignore
+-- LICENSE                        # MIT
+-- README.md
```

## Démarrage rapide
1) Copiez ce dépôt dans `config/` de votre instance Home Assistant.
2) Ouvrez les fichiers `.txt` de `scripts/`, copiez le YAML dans l’éditeur HA (Automations / Scènes / Scripts) ou enregistrez-les sous `.yaml` dans `scripts/`.
3) Ajoutez vos dashboards dans `dashboards/` puis référencez-les dans `configuration.yaml`, par exemple :
   ```yaml
   dashboard: !include dashboards/main.yaml
   ```
4) Placez vos thèmes dans `themes/` et activez-les via Profil > Thème.
5) Rangez vos visuels dans `images/` et mettez à jour leurs chemins dans vos vues.

## Contribution
- Issues et PR bienvenues pour corriger ou ajouter des snippets et de la documentation.
- Avant de soumettre un dashboard ou un thème, supprimez toute référence à des entités privées (`entity_id`) ou à des secrets.
- Conservez un formatage YAML propre (indentation 2 espaces) et ajoutez un court commentaire si le comportement n’est pas évident.

## Sécurité & confidentialité
- Ne versionnez aucun secret (`secrets.yaml`, tokens, mots de passe).
- Adaptez systématiquement les `entity_id` à votre installation avant d’activer un script.
- Les snippets sont fournis “as is” : testez dans un environnement contrôlé avant production.

## Licence
MIT – voir `LICENSE`.
