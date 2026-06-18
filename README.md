# 🧭 Générateur de prompts de planification

Outil **HTML autonome** (un seul fichier, sans dépendance ni build) qui génère, en début de
projet, un prompt de planification de qualité pour Claude (Code ou chat), à partir de
quelques choix.

Pensé pour la **fonction publique** : **100 % local, aucune donnée envoyée** — conforme RGPD
(privacy by design). Aucune requête réseau, aucun CDN, aucun stockage distant.

## Principe directeur — anti-sur-ingénierie

Le risque n'est pas le prompt trop court, c'est le prompt monstrueux et coûteux en tokens.
Règle d'or : *le noyau reste court ; on n'ajoute un module que s'il sert vraiment au projet.*

## Fonctionnalités

- **Noyau (6 blocs, toujours présents)** : cadrage borné, définition du succès, budget de
  contexte, plan spécifique, auto-vérification, ton & efficience.
- **Modules activables (couche 2)** : Claude Code (Plan Mode & orchestration), Vault
  claude-obsidian (+ Graphify), Skills, recherche web conditionnelle, structure du projet,
  garde-fous sécurité, gouvernance / journal de décisions.
- **Paramètres** : Cible (Claude Code · chat), Structure (mono-fichier · modulaire),
  **Envergure du projet** (court · moyen · long terme — pré-coche les modules adaptés),
  mode (blocs activables · prompt complet), langue (FR · EN), format (texte structuré · XML).
- **Panneau Skills** filtré par Cible × Structure : skills perso + skills populaires GitHub.
- **Compteur de tokens** en continu (code couleur, signal anti-sur-ingénierie).
- Ordre d'assemblage **figé** (préserve le prompt caching, prompts comparables d'un projet
  à l'autre), bascule FR/EN et Texte/XML, copier / réinitialiser.

## Utilisation

Ouvrir [`generateur.html`](generateur.html) dans un navigateur (Chrome / Edge / Firefox).
Fonctionne en `file://`, sans serveur. Responsive (utilisable dès 380 px).

Hébergeable sur **GitHub Pages** : une fois Pages activé, l'outil est accessible à
`https://<utilisateur>.github.io/<dépôt>/generateur.html`.

## Technique

- Un seul fichier `generateur.html` : HTML + CSS + JS vanilla, `'use strict'`, zéro dépendance.
- Textes des blocs dans un objet JS éditable (`BLOCKS`), séparé de la logique d'assemblage.
- Catalogue de skills éditable à la main (`SKILLS`), préréglages d'envergure (`PRESET_ENVERGURE`).
