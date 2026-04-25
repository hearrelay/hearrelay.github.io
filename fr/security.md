---
title: Sécurité — HearRelay
lang: fr
---

> La présente version française est fournie à titre de commodité. En cas de divergence ou d'incohérence entre cette version et la version anglaise, la version anglaise prévaut dans la mesure permise par le droit applicable. Cette règle de préséance ne limite pas les droits que vous accorde le droit impératif en matière de protection des consommateurs, de la vie privée ou des données.

# Sécurité

Merci de nous aider à garantir la sécurité des utilisateurs de HearRelay. Cette page explique comment signaler des vulnérabilités et résume la posture de sécurité de HearRelay.

---

## Signaler une vulnérabilité

Veuillez écrire à **hearrelay-security@conex-cp.com** en incluant les informations suivantes :

- Une description claire du problème
- Les étapes pour reproduire (ou une preuve de concept)
- La version de HearRelay et la version d'iOS / iPadOS utilisées
- Toute mesure d'atténuation que vous suggérez
- Si vous souhaitez un crédit public

Nous privilégions l'e-mail pour le signalement initial. Au besoin, nous pouvons mettre en place un **GitHub Security Advisory (divulgation privée)** pour la coordination ultérieure.

**Veuillez ne pas** publier les détails d'une vulnérabilité avant que nous ayons eu l'occasion d'y répondre et de livrer un correctif.

---

## Sphère de sécurité (safe harbor) pour la recherche en sécurité de bonne foi

Nous ne proposons actuellement ni programme de bug bounty ni récompenses monétaires.

Lors de tests ou de signalements de vulnérabilités, veuillez :

- **Ne pas** consulter, modifier, supprimer ou exfiltrer des données qui ne vous appartiennent pas.
- **Ne pas** mener de tests par déni de service, de spam, de hameçonnage, d'ingénierie sociale ni d'attaques physiques.
- **Ne pas** tester sur les services Apple, sur du matériel tiers ou sur tout système qui ne vous appartient pas.
- Limiter les tests à vos propres appareils et à votre propre Apple ID.

Si vous effectuez un signalement de bonne foi dans le cadre de la présente politique et en respectez les règles, **CONEX n'engagera pas intentionnellement de poursuites judiciaires à votre encontre sur la seule base de ce signalement**, sous réserve du droit applicable.

**Limites importantes.** La présente politique **n'autorise pas** l'accès à un quelconque système, service, compte, appareil ou aux données sans permission. Elle **ne renonce à** ni ne limite aucune loi pénale, autorité réglementaire ou droit d'un tiers. Elle **ne lie pas** Apple, GitHub, les fournisseurs de messagerie, les fournisseurs cloud, les services répressifs, les procureurs, les régulateurs ou tout autre tiers.

Nous pouvons prendre les mesures appropriées — y compris notifier les parties concernées ou les autorités — dans les cas impliquant extorsion, menaces, exploitation active, préjudice causé aux utilisateurs, accès non autorisé à des systèmes tiers, ou **manquement substantiel à la présente politique après notification, lorsque le problème peut raisonnablement être corrigé**.

---

## Ce que nous considérons comme couvert

Sont couverts par les signalements :

- L'application HearRelay pour iOS / iPadOS
- La négociation cryptographique HearRelay Secure Channel (X25519 ECDH + P-256 ECDSA + AEAD ChaCha20-Poly1305)
- Le processus de découverte de pairs basé sur iCloud Key-Value Storage
- La gestion locale des fichiers (stockage des enregistrements et suppression automatique)
- Le site Web du projet à `hearrelay.app`

---

## Hors périmètre

- Les vulnérabilités des systèmes d'exploitation, frameworks ou de l'infrastructure iCloud d'Apple — veuillez les signaler directement à Apple
- Les vulnérabilités des routeurs Wi-Fi tiers, des casques Bluetooth ou de tout autre matériel
- Les attaques par ingénierie sociale contre le développeur ou d'autres utilisateurs
- L'absence d'en-têtes de sécurité sur GitHub Pages au-delà de ce que la plateforme nous permet de configurer
- Les problèmes nécessitant un appareil jailbreaké ou autrement compromis

---

## Objectifs de réponse

| Gravité | Première réponse | Résolution visée |
|---|---|---|
| Critique | sous 24 heures | sous 7 jours |
| Élevée | sous 3 jours | sous 30 jours |
| Moyenne / Faible | sous 7 jours | prochaine version régulière |

Il s'agit d'objectifs, et non de garanties.

---

## Divulgation coordonnée

- Nous vous tiendrons informé au fil de l'enquête.
- Nous conviendrons ensemble d'une date de divulgation publique, généralement à la publication d'un correctif.
- À la publication, nous publierons un avis de sécurité et, avec votre accord, vous créditerons.

---

## Résumé de la posture de sécurité

HearRelay est conçue autour de trois principes :

1. **Minimisation des données** — l'audio et les enregistrements ne quittent jamais votre appareil ; aucun SDK d'analytique ni de publicité.
2. **Réseau local uniquement** — les appareils appariés communiquent exclusivement sur le même Wi-Fi / réseau local, jamais via Internet.
3. **Identité cryptographique des pairs** — les appareils s'identifient mutuellement au moyen de clés de signature **P-256** (stockées dans le **Secure Enclave** lorsque celui-ci est pris en charge, avec un repli sur le Keychain), et se découvrent via iCloud Key-Value Storage limité à votre Apple ID.

### Aperçu du flux de données

```text
[Microphone de l'appareil A]
         |
         | traitement local uniquement
         v
[App appareil A] <─── canal chiffré P2P sur le même Wi-Fi ───> [App appareil B]
         |
         | uniquement les métadonnées de découverte d'appareil (clé publique,
         | empreinte, nom de l'appareil, plateforme/modèle, version de l'app,
         | dates de la clé)
         v
[Stockage clé-valeur Apple iCloud, périmètre de l'identifiant Apple]

[Apple App Store + achat intégré]   ─── Apple gère les paiements
[Serveur CONEX]                     ─── aucun
[SDK tiers d'analyse / publicité / suivi]   ─── aucun
```

CONEX n'opère aucun serveur et n'a aucun accès opérationnel aux données stockées dans Apple iCloud ou traitées par Apple IAP. Les seules données que CONEX reçoit directement sont celles que les utilisateurs envoient volontairement par e-mail (voir [Politique de confidentialité §4](/fr/privacy/)).

Le transport utilise le **HearRelay Secure Channel** : échange de clés ECDH X25519 pour une confidentialité persistante, AEAD ChaCha20-Poly1305 avec protection contre la rejouabilité, et nonces dérivés d'un compteur par trame.

Vous pouvez à tout moment effectuer une rotation de la clé d'identité de votre appareil, oublier un appareil pair ou effacer l'ensemble de l'état de sécurité de l'appareil depuis **Réglages → Sécurité** dans l'Application.

Pour une analyse interne plus complète, consultez la documentation de conception du projet.

---

## Contact

- Signalements de sécurité : **hearrelay-security@conex-cp.com**
- Contact général : **hearrelay-support@conex-cp.com**

---

**Traductions disponibles :** [日本語](/ja/security/) · [Français](/fr/security/) · [Español](/es/security/) · [Português (Brasil)](/pt-BR/security/) · [简体中文](/zh-Hans/security/)

Lorsque la présente page est fournie dans une langue autre que l'anglais, la **version anglaise prévaut** dans la mesure permise par le droit applicable. Cette règle de préséance ne limite pas les droits que vous accordent les lois impératives de protection des consommateurs, de la vie privée ou des données de votre pays ou région.
