# Book · Alexis Fayan

Book de mission professionnelle d'**Alexis Fayan**, Project Manager IA & Cloud chez Orange Business
(Cloud Avenue).

**En ligne :** https://book-alexis-fayan.vercel.app

Site statique, un seul fichier `index.html`, zéro dépendance et zéro build. Tout le CSS et le
JavaScript sont dans la page ; les seules ressources externes sont les polices Google Fonts.

## Ce que contient le book

| Section | Contenu |
|---|---|
| Positionnement | La phrase de signature et les trois piliers du profil |
| Preuves chiffrées | 8 indicateurs, chacun adossé à un livrable daté |
| Parcours | Orange Business, Bewizyu, Orange, Barcelone, Epitech |
| Réalisations phares | Formation Avant-Vente Niveau 3, BMS Hub, serveur de démonstration, en onglets contexte / rôle / obstacles / impact |
| Projets d'appui | 9 chantiers complémentaires |
| Compétences | 6 domaines auto-évalués de 1 à 5, marges de progression comprises |
| Méthode | 4 règles de travail |
| Retours | 6 verbatims : manager, experts, formateur, avant-vente, sponsor |
| Formation | Diplômes, certifications, langues |
| Contact | Recherche en cours et moyens de contact |

## Design

**Palette unique**, un papier crème chaud. Le book a d'abord eu deux thèmes ; le sombre a été retiré
pour ne garder qu'une seule identité à maintenir. Le design system correspondant vit sur
claude.ai/design.

Les couleurs ont été calibrées au calcul, pas à l'œil : **tout texte atteint 4,5:1** et toute bordure
de composant interactif 3:1. L'orange de marque `#F16E00` ne dépasse pas 2,67:1 sur ce papier, il
n'est donc jamais utilisé ; le texte orange passe par `#A84C00`, les boutons, jauges et puces par
`#BD5600`.

La séparation visuelle vient du remplissage (carte blanche sur papier crème) plutôt que d'un cerclage.

## Fonctionnement

- **Sans JavaScript, tout le contenu reste visible.** Les animations d'apparition ne s'activent que si
  la classe `js` a été posée sur `<html>`, ce que seul le script fait.
- Aucune bascule de thème : une seule palette, aucun état à mémoriser.
- Les animations respectent `prefers-reduced-motion`.
- **Export PDF** : le bouton « Enregistrer ce book en PDF » ouvre la boîte d'impression. La feuille
  `@media print` déplie les onglets, repasse en fond blanc, force un saut de page avant chaque étude de
  cas et affiche les URL des liens externes.
- **Responsive** de 360 px à 1440 px, sans débordement horizontal.
- Accessibilité : lien d'évitement, motif ARIA `tablist` complet, menu mobile modal qui pose `inert` sur
  le reste de la page, focus visible partout.

## Confidentialité

Le book est public. Les noms de tiers (collègues, clients, prospects), les montants d'affaires, les
références de tickets internes et les prix de l'offre sont volontairement anonymisés ou généralisés.
Seul Christophe Thomas est cité nommément, en tant que signataire d'une lettre de recommandation
destinée aux recruteurs. La lettre elle-même n'est pas hébergée ici : elle est communiquée sur demande.

## Fichiers

```
index.html                    le book, un seul fichier
favicon.svg                   monogramme AF, aplat plein
robots.txt / sitemap.xml
vercel.json                   cleanUrls, cache des assets, en-têtes de sécurité
assets/alexis-fayan.jpg       portrait
assets/apple-touch-icon.png   icône iOS
assets/og.jpg                 image de partage (LinkedIn, réseaux sociaux)
assets/hub-hero.jpg           BMS Hub, page d'accueil publique
assets/hub-piliers.jpg        BMS Hub, les quatre besoins couverts
assets/hub-domaines.jpg       BMS Hub, entrée par domaine
assets/hub-dashboard.jpg      BMS Hub, tableau de bord connecté
assets/hub-formation.jpg      BMS Hub, parcours de formation
assets/hub-changelog.jpg      BMS Hub, journal des versions
```

## Déploiement

Le projet est déployé sur Vercel comme site statique (aucun framework, aucune commande de build).
Le projet Vercel **n'est pas relié au dépôt Git** : pousser sur `main` ne redéploie pas. La mise en
production se fait avec `npx vercel --prod` depuis ce dossier.

## Contact

- LinkedIn : https://www.linkedin.com/in/alexis-fayan/
- GitHub : https://github.com/AlexisFayan
- Email : fayanalexis@gmail.com
