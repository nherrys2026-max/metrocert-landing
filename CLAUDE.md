# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Projet

MetroCert (cours GET 409) : générateur de certificats d'étalonnage multi-instruments et multi-sociétés, conforme à l'ISO/IEC 17025:2017. Porté par Ivon NKOUNKOU, chef de produit. Ce dépôt ne contient que la landing page (HTML/CSS statique, sans build, tests ni lint) ; le produit et les livrables sont dans `nherrys2026-max/Get409-metrocert`.

**Persona :** Mame Diarra, responsable technique d'un laboratoire d'étalonnage à Dakar. Elle jongle avec un modèle de certificat différent par famille d'instruments et par client.

**HMW définitif (S2) :** « Comment pourrions-nous permettre aux responsables techniques de laboratoires d'étalonnage au Sénégal, comme Mame Diarra, qui jonglent avec un modèle de certificat différent par famille d'instruments et par client, de passer des relevés de mesure à un certificat conforme à l'ISO/IEC 17025 sans aucune ressaisie, afin de livrer leurs clients dans la journée et de passer leurs audits d'accréditation sans écart lié aux certificats ? »

## Règles

- Tout est en français : pages, commentaires, commits, documentation.
- Les données sont fictives et toujours signalées (pied de page « Prototype pédagogique GET 409 — données fictives »).
- Citer l'ISO/IEC 17025:2017 sans jamais inventer de numéro d'accréditation.
- Pages lisibles à 360 px ; `min-width: 0` sur les enfants de grille et de flex.
- **v2 est la direction retenue** : toute évolution part de `v2/`. `v1/` est conservée pour la comparaison.

## Structure

- `v1/index.html` : version sans skill de design. `v2/index.html` : version `frontend-design` (règle graduée, étiquette d'étalonnage, Barlow).
- `index.html` (racine) redirige vers `v2/`. `COMPARAISON.md` décrit les écarts v1/v2.
- Pages autonomes (CSS dans `<style>`). Le contenu est dupliqué : un changement de texte se fait dans v1 et v2.
- Bouton « Demander un étalonnage » → `https://metrocert.netlify.app/contact`. Contacts fictifs : contact@metrocert.sn, +221 33 000 00 00.

## Déploiement

Dépôt public `nherrys2026-max/metrocert-landing`, GitHub Pages sur `master` (racine) : https://nherrys2026-max.github.io/metrocert-landing/. Un push redéploie. `gh` est absent du PATH de Git Bash : utiliser `C:\Program Files\GitHub CLI\gh.exe` via PowerShell.
