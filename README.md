# Book — Alexis Fayan

Book / portfolio en ligne d'**Alexis Fayan**, Project Manager IA & Cloud chez Orange Business (Cloud Avenue).

**En ligne :** https://book-alexis-fayan.vercel.app

Site statique, un seul fichier `index.html`, zéro dépendance et zéro build. Tout le CSS et le JavaScript
sont dans la page ; les seules ressources externes sont les polices Google Fonts.

## Ce que contient le book

| Section | Contenu |
|---|---|
| Positionnement | La phrase de signature et les trois piliers du profil |
| Preuves chiffrées | Huit indicateurs, chacun adossé à un livrable daté |
| Parcours | Orange Business, Bewizyu, Orange, Barcelone, Epitech |
| Réalisations phares | Formation Avant-Vente Niveau 3, BMS Hub, serveur de démonstration (onglets contexte / rôle / obstacles / impact) |
| Projets d'appui | Neuf chantiers complémentaires |
| Compétences | Six domaines auto-évalués de 1 à 5, marges de progression comprises |
| Méthode | Quatre règles de travail |
| Retours | Verbatims de managers, experts, formateurs et avant-ventes |
| Formation | Diplômes, certifications, langues |
| Contact | Recherche en cours et moyens de contact |

## Fonctionnement

- **Thème sombre par défaut**, thème clair via le bouton de la barre de navigation (préférence mémorisée
  dans `localStorage`).
- **Dégradation propre** : sans JavaScript, les chiffres, les barres de niveau et le contenu des onglets
  restent lisibles. Les animations respectent `prefers-reduced-motion`.
- **Export PDF** : le bouton « Enregistrer ce book en PDF » ouvre la boîte d'impression ; une feuille de
  style `@media print` déplie les onglets, passe en fond blanc et affiche les URL des liens.
- **Responsive** vérifié de 360 px à 1440 px, sans débordement horizontal.

## Confidentialité

Le book est public. Les noms de tiers (collègues, clients, prospects), les montants d'affaires, les
références de tickets internes et les prix de l'offre sont volontairement anonymisés ou généralisés.
Seul Christophe Thomas est cité nommément, en tant que signataire d'une lettre de recommandation
destinée aux recruteurs. La lettre elle-même n'est pas hébergée ici : elle est communiquée sur demande.

## Fichiers

```
index.html              le book
favicon.svg             monogramme AF
robots.txt / sitemap.xml
vercel.json             cleanUrls, cache des assets, en-têtes de sécurité
assets/alexis-fayan.png portrait
assets/bms-hub.jpg      capture de la page d'accueil publique de BMS Hub
assets/og.jpg           image de partage (LinkedIn, réseaux sociaux)
```

## Déploiement

Le projet est déployé sur Vercel comme site statique (aucun framework, aucune commande de build).
Toute modification de `index.html` poussée sur `main` peut être redéployée depuis le tableau de bord
Vercel, ou directement via `vercel --prod`.

## Contact

- LinkedIn : https://www.linkedin.com/in/alexis-fayan/
- GitHub : https://github.com/AlexisFayan
- Email : fayanalexis@gmail.com
