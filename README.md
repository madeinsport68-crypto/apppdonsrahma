# Code source - Borne de Dons Mosquée (Zettle Reader 2)

Ce dossier contient l'ossature pour mettre en place une borne tactile de dons sous **Next.js (App Router)** couplée avec l'API **Reader Connect** de Zettle.

## Structure des fichiers fournis
- `src/app/page.tsx` : L'interface tactile (v0 style) incluant le pavé numérique, les montants rapides et la gestion des différents statuts d'affichage (Attente de carte, Succès, Échec).
- `src/app/api/donate/route.ts` : La fonction Backend sécurisée s'exécutant côté serveur pour l'obtention du token OAuth 2.0 et l'initiation du paiement REST vers Zettle.
- `.env.local.example` : Le fichier modèle pour vos variables d'environnement secrètes à configurer sur Vercel.

## Déploiement et Configuration
1. Glissez les fichiers correspondants dans votre projet Next.js connecté à votre dépôt **GitHub**.
2. Récupérez vos clés API sur le [Zettle Developer Portal](https://developer.zettle.com/).
3. Ajoutez vos clés `ZETTLE_CLIENT_ID` et `ZETTLE_CLIENT_SECRET` dans les **Environment Variables** de votre projet sur **Vercel**.
