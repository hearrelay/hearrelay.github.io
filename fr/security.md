---
title: Sécurité — HearRelay
lang: fr
---

# Sécurité

Merci de nous aider à garantir la sécurité des utilisateurs de HearRelay. Cette page explique comment signaler une vulnérabilité et résume la posture de sécurité de HearRelay.

> Cette traduction est fournie à titre de commodité. En cas de divergence avec la [version anglaise](/en/security/), la version anglaise prévaut.

---

## Signaler une vulnérabilité

Envoyez un e-mail à **hearrelay-security@conex-cp.com** en incluant :

- Une description claire du problème
- Les étapes pour reproduire (ou une preuve de concept)
- La version de HearRelay et la version d'iOS / iPadOS utilisées
- Toute mesure d'atténuation suggérée
- Si vous souhaitez un crédit public

Nous privilégions l'e-mail pour le signalement initial. Au besoin, nous pouvons mettre en place un **GitHub Security Advisory (divulgation privée)** pour la coordination ultérieure.

**Veuillez ne pas** publier les détails d'une vulnérabilité avant que nous ayons eu l'occasion de répondre et de livrer un correctif.

---

## Ce que nous considérons comme couvert

Sont couverts par les signalements :

- L'application HearRelay pour iOS / iPadOS
- La négociation cryptographique et le transport TLS utilisés entre les appareils appariés
- Le processus de découverte de pairs basé sur iCloud Key-Value Storage
- La gestion locale des fichiers (stockage des enregistrements et suppression automatique)
- Le site Web du projet à `hearrelay.github.io`

---

## Hors périmètre

- Les vulnérabilités des systèmes d'exploitation, frameworks ou infrastructure iCloud d'Apple — veuillez les signaler directement à Apple
- Les vulnérabilités des routeurs Wi-Fi, des casques Bluetooth ou du matériel tiers
- Les attaques par ingénierie sociale contre le développeur ou les autres utilisateurs
- L'absence d'en-têtes de sécurité sur GitHub Pages au-delà de ce que la plateforme nous permet de configurer
- Les problèmes ne se reproduisant que sur un appareil jailbreaké ou autrement compromis

---

## Objectifs de réponse

| Gravité | Première réponse | Résolution visée |
|---|---|---|
| Critique | sous 24 heures | sous 7 jours |
| Élevée | sous 3 jours | sous 30 jours |
| Moyenne / Faible | sous 7 jours | prochaine version régulière |

Il s'agit d'objectifs, non de garanties.

---

## Divulgation coordonnée

- Nous vous tiendrons informé au fil de l'enquête.
- Nous conviendrons ensemble d'une date de divulgation publique, généralement à la publication d'un correctif.
- À la publication, nous publierons un avis de sécurité et, avec votre accord, vous créditerons.

---

## Résumé de la posture de sécurité

HearRelay est conçue autour de trois principes :

1. **Minimisation des données** — aucun son ni enregistrement ne quitte votre appareil ; aucun SDK d'analytique ni de publicité.
2. **Uniquement sur le réseau local** — les appareils appariés communiquent exclusivement sur le même Wi-Fi / réseau local, jamais via Internet.
3. **Identité cryptographique des pairs** — les appareils s'identifient mutuellement via des clés **Curve25519 / P-256**, protégées dans le **Secure Enclave** lorsque c'est possible, et découvertes via iCloud Key-Value Storage limité à votre identifiant Apple.

Le transport est chiffré avec **TLS 1.3** en n'utilisant que les suites AEAD fournies par iOS.

Pour une analyse plus approfondie, consultez la documentation de conception du projet.

---

## Contact

- Signalements de sécurité : **hearrelay-security@conex-cp.com**
- Contact général : **hearrelay-support@conex-cp.com**

---

**English version:** [Security](/en/security/)
