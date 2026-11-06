# Hébergement Cloudflare depuis GitHub

Source : antl-rch/le-podium-pole-dance. Branche de production : main.

Build : npm run build:cloudflare ; sortie : dist. Le build exécute les vérifications disponibles dans le projet. Aucun téléversement manuel de dist.

Variables publiques : NODE_VERSION=24.22.1, DEPLOY_TARGET=cloudflare, VITE_HOSTING_PLATFORM=cloudflare, VITE_PAYMENTS_ENABLED=false. CLOUDFLARE_BUILD_PREVIEW=true impose noindex pendant la validation et sera ajusté au moment de la bascule publique. Aucun secret serveur dans Vite.

Projet Cloudflare Git configuré : antl-podium. Les anciennes sources et adresses GitHub Pages restent disponibles pendant la migration. Le chemin de base historique reste conservé lorsque DEPLOY_TARGET ne vaut pas cloudflare.

Adresse de validation : https://antl-podium.pages.dev/ . Aucun domaine de production associé pendant la recette.
