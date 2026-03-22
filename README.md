# Priorit — Organisateur de tâches intelligent

> Saisie libre · Matrice d'Eisenhower · Google Calendar

![PWA](https://img.shields.io/badge/PWA-installable-blueviolet)
![Claude API](https://img.shields.io/badge/Powered%20by-Claude%20API-e8d5a3)
![License](https://img.shields.io/badge/license-MIT-green)

---

## À propos

**Priorit** est une Progressive Web App (PWA) installable sur Android (et desktop) qui permet de :

1. **Saisir des tâches en texte libre** — vous écrivez comme vous pensez
2. **Laisser l'IA les classer automatiquement** selon la matrice d'Eisenhower
3. **Les ajouter en un clic dans Google Calendar**

---

## Fonctionnalités

- ✍️ Saisie en langage naturel (pas de formulaire)
- 🧠 Classement automatique par IA (Claude Sonnet)
- 📊 Matrice d'Eisenhower en 4 quadrants (Q1 → Q4)
- 🗂️ 6 catégories personnalisées avec ordre de priorité
- 📅 Ajout direct dans Google Calendar via MCP
- 📱 PWA installable sur Android (icône sur le bureau)
- ⚡ Interface mobile-first, rapide et minimaliste

---

## Ordre de priorité des catégories

| Rang | Catégorie |
|------|-----------|
| 1 | Finances / administratif |
| 2 | Famille / proches |
| 3 | Santé / RDV médicaux |
| 4 | Projets personnels |
| 5 | Loisirs / voyages |
| 6 | Courses / quotidien |

---

## Matrice d'Eisenhower

| | Urgent | Pas urgent |
|---|---|---|
| **Important** | 🔴 Q1 — Faire maintenant | 🟠 Q2 — Planifier |
| **Pas important** | 🟡 Q3 — Déléguer | 🟢 Q4 — Plus tard |

---

## Installation sur Android

1. Hébergez ce dépôt sur **GitHub Pages** (Settings → Pages → `main` branch)
2. Ouvrez l'URL `https://Koka-sklearn.github.io/priorit` dans **Chrome Android**
3. Chrome affiche une bannière **"Ajouter à l'écran d'accueil"**
4. Tapez **Installer** → l'icône apparaît sur votre bureau 🎉

---

## Stack technique

- HTML / CSS / JavaScript vanilla
- [Claude API](https://www.anthropic.com) (claude-sonnet-4) pour l'analyse IA
- Google Calendar MCP pour la création d'événements
- Service Worker pour le mode offline
- Web App Manifest pour l'installation PWA

---

## Structure du projet

```
priorit/
├── index.html       # App principale (mobile-first)
├── manifest.json    # Config PWA (nom, icônes, couleurs)
├── sw.js            # Service Worker (cache offline)
└── icons/           # Icônes PWA (72px → 512px)
```

---

## Lancement local

Aucune dépendance. Servez simplement les fichiers avec un serveur local :

```bash
# Python
python3 -m http.server 8000

# Node
npx serve .
```

Puis ouvrez `http://localhost:8000`

> ⚠️ La PWA nécessite HTTPS pour être installable. GitHub Pages fournit HTTPS automatiquement.

---

*Développé avec [Claude](https://claude.ai) — Anthropic*
