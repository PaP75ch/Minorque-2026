# 🏝️ Minorque 2026 — La plateforme du voyage

Plateforme web collaborative pour notre semaine à Minorque (25 juillet → 1er août 2026) :
programme jour par jour, plages & restaurants avec itinéraires, carte interactive,
budget partagé entre les 3 couples, votes et commentaires.

**10 voyageurs** : Anne-Sophie & Stephen (William, 8 ans) · Céline & Cédric (Nathan & Raphaël) · Pierre-Alexandre & Amandine (Apolline, 1 an ½)

---

## 🚀 Mettre en ligne en 5 minutes (GitHub Pages — gratuit)

1. Créez un compte sur [github.com](https://github.com) si besoin
2. Cliquez **New repository** → nommez-le `minorque-2026` → **Public** → Create
3. Cliquez **uploading an existing file** et glissez **tous les fichiers de ce dossier**
   (`index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`)
4. **Commit changes**
5. Allez dans **Settings → Pages** → Source : `Deploy from a branch` → Branch : `main` / `(root)` → **Save**
6. Après ~1 minute, votre lien apparaît :
   **`https://VOTRE-PSEUDO.github.io/minorque-2026/`**

➡️ C'est **ce lien** que vous partagez au groupe WhatsApp. Photos réelles,
carte interactive et itinéraires Google Maps fonctionnent à 100 %.

## 📱 Déjà une application mobile (PWA)

Le site est une **Progressive Web App** : une fois le lien ouvert sur téléphone,
chacun peut l'**installer sur son écran d'accueil** comme une vraie app :

- **iPhone (Safari)** : bouton Partager → « Sur l'écran d'accueil »
- **Android (Chrome)** : menu ⋮ → « Ajouter à l'écran d'accueil » (ou bannière automatique)

L'app s'ouvre alors en plein écran avec son icône 🏝️, et le service worker
garde la dernière version consultable **même sans réseau** (pratique à la plage).

## 🛠️ Aller plus loin (vraie app native)

Si vous voulez plus tard une app sur l'App Store / Play Store :

- **Capacitor** (recommandé) : `npx cap init` puis `npx cap add ios android`
  — il enveloppe ce même `index.html` dans une app native
- Les données partagées (votes, budget) nécessiteraient alors un petit backend
  (Firebase / Supabase gratuit) à la place du stockage local

## 📂 Structure

| Fichier | Rôle |
|---|---|
| `index.html` | Toute la plateforme (HTML + CSS + JS, autonome) |
| `manifest.webmanifest` | Identité de l'app (nom, icônes, couleurs) |
| `sw.js` | Service worker — mode hors-ligne |
| `icon-192/512.png` | Icônes d'installation |

*Fes-ho bé — bon voyage tous les dix ! ✦*
