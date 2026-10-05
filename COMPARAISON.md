# Comparaison v1 / v2

Même contenu, même lien du bouton, une seule page chacune, lisibles à 360 px (`min-width: 0` sur les éléments de grille et de flex).

| Aspect | v1 (sans skill) | v2 (skill frontend-design) |
|---|---|---|
| Démarche | Écrite directement, sans plan | Plan de design (palette, typographie, composition) vérifié avant le code |
| Univers visuel | Générique « entreprise » : bandeau bleu, cartes grises | Métrologie : règle graduée en CSS, étiquette d'étalonnage, planche de lecture |
| Palette | Bleu, orange, gris neutres | Gris acier, bleu pétrole, vert « conforme », orange signal réservé au bouton |
| Typographie | Arial système | Barlow Condensed (titres) + Barlow (texte), échelle fluide `clamp()` |
| Hero | Texte centré sur aplat bleu | Titre à gauche, étiquette d'étalonnage inclinée portant les 3 chiffres |
| Chiffres | 3 cartes identiques | Lignes d'une étiquette (champ / valeur) |
| Prestations | 5 cartes identiques | Planche de lecture : une ligne par grandeur, avec description |
| Étapes | Liste numérotée simple | Trois colonnes numérotées, repère épais en tête |
| Secteurs | Pastilles grises | Pastilles à contour marqué, en typographie condensée |
| Contact | Paragraphe simple | Bloc sombre pleine largeur, liens en grand |
| Accessibilité | Correcte, sans focus dédié | Focus visible, `prefers-reduced-motion`, contrastes vérifiés |
| Dépendances | Aucune | Polices Google Fonts (avec repli sur Arial Narrow / Arial) |
| Contenu ajouté | Descriptions d'étapes courtes | Descriptions d'instruments par prestation (texte fictif) |

## À retenir

v1 est correcte et fonctionnelle, mais pourrait être celle de n'importe quelle PME. v2 se reconnaît comme celle d'un laboratoire de métrologie, au prix d'un peu plus de CSS et d'une police externe.
