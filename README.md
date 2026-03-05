# TechEnClair – Ressources Home Assistant

Ensemble de snippets et ressources pour personnaliser Home Assistant : scripts prêts à copier, dossier pour vos dashboards, thèmes et visuels.

## Arborescence
```
TechEnClair/
+-- .gitignore
+-- LICENSE
+-- README.md
+-- custom-cards/
¦   +-- instructions.md
+-- dashboards/            # placez ici vos vues Lovelace (.yaml)
+-- images/
¦   +-- Poubelle.webp
+-- scripts/
¦   +-- automation-examples.yaml
¦   +-- 4 Personnage cote a cote.txt
¦   +-- Alexa Annonce.txt
¦   +-- Alexa Minuteur.txt
¦   +-- boite au lettre.txt
¦   +-- Bouton Simulation présence.txt
¦   +-- Colonne Lumière avec swipe.txt
¦   +-- Lave vaisselle.txt
¦   +-- Lumières.txt
¦   +-- Meteo animé V2.txt
¦   +-- Média PLAYER.txt
¦   +-- Météo.txt
¦   +-- poubelle.txt
¦   +-- PRISE ANIMATION.txt
¦   +-- Script APPLE TV Télécommande.txt
¦   +-- Script cinema.txt
¦   +-- Script Conso.txt
¦   +-- Script COURSES.txt
¦   +-- Script emploi du temps.txt
¦   +-- Script Extérieur FREEBOX.txt
¦   +-- Script MESSAGE ENFANTS.txt
¦   +-- TEMPO DESIGN.txt
¦   +-- Theme PS5 LECTURE EN COURS.txt
¦   +-- Thème Xbox.txt
¦   +-- TUTO SONNETTE PLEIN ECRAN.txt
¦   +-- Tuto Wifi avatar.txt
+-- themes/                # placez ici vos thèmes (.yaml)
```

## Utilisation rapide
1) Copier le dépôt dans `config/` de Home Assistant.
2) Pour chaque snippet `.txt`, ouvrez-le et copiez le YAML dans l’éditeur Home Assistant (Automations/Scènes/Scripts) ou enregistrez-le sous `.yaml` dans `scripts/`.
3) Ajoutez vos dashboards dans `dashboards/` puis référencez-les dans `configuration.yaml` (ex. `dashboard: !include dashboards/main.yaml`).
4) Déposez vos thèmes dans `themes/` et activez-les via Profil > Thème.
5) Placez vos visuels (icônes, captures) dans `images/` et mettez à jour les chemins dans vos vues.

## Notes
- `custom-cards/instructions.md` contient les prérequis pour certaines cartes Lovelace.
- Les dashboards et thèmes fournis sont vides par défaut : ajoutez vos propres fichiers.

## Sécurité
- Ne versionnez aucun secret (`secrets.yaml`, tokens, mots de passe).
- Vérifiez et adaptez les `entity_id` avant d’activer un script.
