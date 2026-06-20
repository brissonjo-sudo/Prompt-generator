# Déclaration d'accessibilité

> **Gabarit à compléter par l'entité qui déploie l'outil.** Les champs entre `{ }` doivent être
> renseignés. L'auto-évaluation technique ci-dessous est fournie par les auteurs de l'outil ; elle
> ne vaut pas audit de conformité par un tiers. Pour une conformité RGAA opposable, faire réaliser
> un audit par un prestataire qualifié, puis publier cette déclaration sur la page de l'outil.

**{Nom de l'organisme}** s'engage à rendre son service numérique accessible, conformément à
l'article 47 de la loi n° 2005-102 du 11 février 2005 et au décret n° 2019-768 du 24 juillet 2019.

Cette déclaration d'accessibilité s'applique à : **Générateur de prompts de planification**
(`generateur.html`) — {URL de déploiement}.

## État de conformité

Le service est **{non conforme / partiellement conforme / totalement conforme}** avec le
**Référentiel général d'amélioration de l'accessibilité (RGAA), version 4.1**.

> Auto-évaluation des auteurs (avant audit tiers) : **partiellement conforme** — aucune
> non-conformité bloquante connue n'a été identifiée sur le périmètre testé, mais l'absence
> d'audit externe interdit de déclarer une conformité totale.

## Résultats des tests

{À compléter après audit : taux de conformité = X %, sur N critères applicables.}

## Contenus non accessibles

### Non-conformités

{Lister les éventuelles non-conformités relevées lors de l'audit, ou « Aucune non-conformité
connue à ce jour » si l'auto-évaluation n'en a pas relevé.}

### Dérogations pour charge disproportionnée

Néant.

### Contenus non soumis à l'obligation d'accessibilité

Néant.

## Mesures d'accessibilité mises en œuvre (auto-évaluation technique)

- **Structure et repères** : page avec langue déclarée (`lang="fr"`), titre de page explicite,
  un seul `h1`, panneaux titrés (`h2`), groupes de champs en `fieldset`/`legend`, listes
  exposées (`role="list"`), repères ARIA sur les régions, lien d'évitement vers l'aperçu.
- **Couleurs et contrastes** : tous les textes et pastilles d'état présentent un contraste
  ≥ 4,5:1. L'information de coût (compteur de tokens) n'est pas portée par la seule couleur
  (marqueur `✓ / ⚠ / ⛔` + libellé textuel pour les lecteurs d'écran).
- **Clavier** : toutes les fonctions sont accessibles au clavier ; focus visible renforcé sur
  les boutons, liens et contrôles segmentés ; aucun piège au clavier.
- **Lecteurs d'écran** : étiquettes associées aux champs, emojis décoratifs masqués
  (`aria-hidden`), changement de langue du contenu généré annoncé (`lang` dynamique sur
  l'aperçu), confirmation de copie annoncée via une région `role="status"`.
- **Confort** : respect de `prefers-reduced-motion`, mise en page responsive jusqu'à 380 px,
  unités relatives (`rem`) permettant l'agrandissement des textes.

## Établissement de cette déclaration

Déclaration établie le **{date}**.

- Référentiel : **RGAA 4.1**.
- Méthode : {auto-évaluation des auteurs / audit réalisé par {prestataire}}.
- Technologies utilisées : HTML, CSS, JavaScript (aucune dépendance, aucune requête réseau).
- Outils d'évaluation : {ex. inspection du code, mesure de contrastes, lecteur d'écran NVDA/VoiceOver}.
- Pages testées : `generateur.html` (page unique).

## Retour d'information et contact

Si vous ne parvenez pas à accéder à un contenu ou à un service, vous pouvez contacter le
responsable pour être orienté vers une alternative accessible ou obtenir le contenu sous une
autre forme :

- Contact : **{nom / e-mail / formulaire}**.

## Voies de recours

Si vous constatez un défaut d'accessibilité vous empêchant d'accéder à un contenu ou une
fonctionnalité du service, que vous nous le signalez et que vous ne parvenez pas à obtenir une
réponse, vous êtes en droit de faire parvenir vos doléances ou une demande de saisine au
Défenseur des droits :

- Formulaire : https://formulaire.defenseurdesdroits.fr/
- Liste des délégués de votre région avec leurs coordonnées : https://www.defenseurdesdroits.fr/saisir/delegues
- Par courrier (gratuit, sans timbre) : Défenseur des droits, Libre réponse 71120, 75342 Paris CEDEX 07.
