# TechEnClair – Home Assistant Dashboards
Trois dashboards prêts à l’emploi (principal, énergie, mobile) + thème dédié.

## Installation rapide
1. Copier ce dossier dans `config/` de Home Assistant.
2. Dans `configuration.yaml`, inclure :
   dashboard: !include dashboards/main-dashboard.yaml
3. Recharger l’interface ou redémarrer.
4. Activer le thème : Profil > Thème > TechEnClair.

## Aperçus
- images/preview-main.png
- images/preview-mobile.png

## Contenu
- dashboards/main-dashboard.yaml – vue complète maison.
- dashboards/energy-dashboard.yaml – suivi énergie.
- dashboards/mobile-dashboard.yaml – vue mobile compacte.
- themes/techenclair-theme.yaml – palette et fonds.
- scripts/automation-examples.yaml – automations d’exemple.
- custom-cards/instructions.md – cartes/custom components suggérés.

## Sécurité
- Ne versionner aucun secret (`secrets.yaml`).
- Adapter les `entity_id` à votre installation.
