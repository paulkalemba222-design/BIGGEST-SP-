# BIGGEST SP — Powered by PAUL AI

Version initiale connectée au projet Supabase existant.

## Fichiers
- `index.html`, `style.css`, `app.js` : interface et logique du site.
- `config.js` : URL du projet et publishable key publique.
- `manifest.json` : métadonnées PWA.

## Fonctionnalités branchées
- Inscription par e-mail et mot de passe, connexion et déconnexion via Supabase Auth.
- Chargement du profil de l'utilisateur.
- Création de conversations personnelles.
- Chargement, envoi et abonnement temps réel aux messages Supabase (selon la configuration Realtime du projet).
- Modification du nom affiché.

## Projet Supabase utilisé
`https://agiezrhpcdmhgxwqsbmb.supabase.co`

La clé dans `config.js` est une publishable key prévue pour le navigateur. Ne jamais y placer une clé `service_role` ou une clé `secret`.

## Déploiement
Importer le contenu du dossier `BIGGEST_SP_BASE` dans le dépôt GitHub connecté au projet Vercel `biggestsp`. Vérifier que le répertoire publié contient `index.html` à sa racine, puis déployer.

## Limites honnêtes
Cette version n'est pas une messagerie complète équivalente à WhatsApp. La création d'une conversation ne permet encore que d'y accéder depuis le compte créateur; l'ajout sécurisé d'autres utilisateurs et groupes demande une prochaine étape côté backend/RLS. Les statuts sont encore locaux. Les appels audio/vidéo, notifications push, chiffrement de bout en bout et l'intégration PAUL AI ne sont pas inclus. L'inscription peut nécessiter une confirmation e-mail selon les réglages Supabase.
