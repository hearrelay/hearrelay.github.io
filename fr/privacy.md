---
title: Politique de confidentialité — HearRelay
lang: fr
---

> La présente version française est fournie à titre de commodité. En cas de divergence ou d'incohérence entre cette version et la version anglaise, la version anglaise prévaut dans la mesure permise par le droit applicable. Cette règle de préséance ne limite pas les droits que vous accorde le droit impératif en matière de protection des consommateurs, de la vie privée ou des données.

# Politique de confidentialité

**Date d'entrée en vigueur : 2026-04-25**
**Dernière mise à jour : 2026-04-25**

HearRelay (« l'Application ») est conçue pour respecter la vie privée par défaut. La présente politique explique quelles données sont, et ne sont pas, traitées lorsque vous utilisez HearRelay.

Pour toute question, veuillez nous contacter à l'adresse **hearrelay-privacy@conex-cp.com**.

---

## 1. Qui nous sommes

HearRelay est développée par **CONEX Corporation** (株式会社CONEX), une société constituée au Japon (« l'Éditeur », « nous », « CONEX »). L'Application est conçue de telle sorte que les sons, les enregistrements, les informations de paiement, les identifiants publicitaires, les données analytiques et les données de suivi ne soient pas transmis aux serveurs de CONEX. CONEX n'exploite aucun serveur dorsal pour l'Application.

Dans la mesure où des informations limitées de découverte d'appareils sont traitées par Apple au sein de votre compte Apple ID (voir §4), CONEX n'a pas accès à ce traitement et ne l'opère pas. Lorsque le droit applicable considère néanmoins ces informations comme des « données personnelles », CONEX coopère de bonne foi avec les demandes d'informations conformément au §10.

Pour toute correspondance, veuillez utiliser les adresses e-mail figurant en bas de cette page.

---

## 2. Données que nous ne collectons pas

CONEX **ne collecte ni ne reçoit** sur ses propres serveurs, ne stocke et ne partage aucune des données suivantes :

- Sons captés par le microphone de votre appareil
- Enregistrements audio que vous créez avec l'Application
- Coordonnées, localisation, photos, données caméra ou identifiants d'appareil
- Identifiants publicitaires (IDFA, IDFV utilisés à des fins de suivi)
- Données analytiques, télémétrie de plantage acheminée vers des services tiers ou profils comportementaux
- Numéros de carte de paiement ou informations de facturation (Apple traite les achats — voir §7)

HearRelay ne contient aucun SDK tiers d'analytique, de publicité ou de suivi.

---

## 3. Données traitées localement sur votre appareil

L'Application traite les éléments suivants sur votre appareil, et **uniquement sur votre appareil** :

| Donnée | Finalité | Conservation |
|---|---|---|
| Audio du microphone (en direct) | Surveillance en temps réel via un casque ou un appareil apparié sur le même Wi-Fi | Non stocké |
| Enregistrements audio (optionnel) | Vous pouvez enregistrer manuellement des sessions | Supprimés automatiquement après 24 heures par défaut ; vous pouvez prolonger ou supprimer plus tôt |
| Historique de connexion (nom du pair, date de dernière connexion) | Fonction de commodité pour se reconnecter rapidement | Stocké localement ; effacé lors de la désinstallation de l'Application |
| Préférences de l'application (y compris la date de début de la période d'essai pour le déclenchement de l'achat) | Mémoriser vos réglages | Stockées localement |

Lorsque vous désinstallez l'Application, toutes les données ci-dessus sont supprimées avec elle.

---

## 4. Informations limitées traitées par Apple iCloud (périmètre Apple ID)

Pour permettre à vos propres appareils Apple de se découvrir mutuellement sur le même Wi-Fi, l'Application fait en sorte que les informations limitées de découverte d'appareils suivantes soient stockées dans **Apple iCloud Key-Value Storage** au sein de votre compte Apple ID :

- Une **clé publique** cryptographique générée sur votre appareil
- Une **empreinte SHA-256** de cette clé publique
- Le **nom** de votre appareil (tel que défini dans Réglages iOS → Général → Informations → Nom)
- La **plateforme**, le **modèle** de votre appareil et la **version de l'application** installée
- La **date de création** et la **date de dernière rotation** de la clé

Ces informations sont stockées dans le périmètre de votre propre Apple ID, au sein du service iCloud d'Apple, et ne sont visibles ni par d'autres titulaires d'Apple ID, ni par CONEX. CONEX n'exploite pas Apple iCloud et n'accède pas à ces informations sur ses propres serveurs. Le traitement par Apple est régi par la politique de confidentialité d'Apple et les conditions iCloud.

**Selon le droit applicable et les paramètres de nom de votre appareil, certaines de ces informations peuvent être considérées comme des données personnelles** — par exemple, si le nom de votre appareil contient votre nom complet. Nous les décrivons ici par souci de transparence. Vous pouvez modifier le nom de votre appareil à tout moment dans les Réglages iOS, et vous pouvez purger l'identité de l'Application (en effectuant une rotation de sa clé et en supprimant l'entrée) depuis **Réglages → Sécurité → Réinitialiser toute la sécurité de l'appareil** dans l'Application.

---

## 5. Communications réseau

HearRelay communique **uniquement** avec d'autres appareils Apple qui sont :

1. Connectés au même Apple ID, **et**
2. Connectés au même Wi-Fi / réseau local

Les communications sont chiffrées au moyen du **HearRelay Secure Channel** (échange de clés ECDH X25519 + AEAD ChaCha20-Poly1305 avec protection contre la rejouabilité). HearRelay **n'envoie aucune** donnée via Internet vers des serveurs distants et ne prend pas en charge la surveillance à distance entre réseaux. L'usage à distance est délibérément interdit afin de prévenir toute surveillance dissimulée.

---

## 6. Enregistrements audio que vous créez

Si vous activez la fonction d'enregistrement :

- Les enregistrements sont sauvegardés **uniquement sur l'appareil qui les a créés**
- Les enregistrements sont stockés à l'intérieur du bac à sable de l'Application avec un **chiffrement au niveau fichier** (`NSFileProtectionComplete`)
- Les enregistrements sont **automatiquement supprimés 24 heures** après leur création, sauf si vous choisissez explicitement de les conserver
- Vous pouvez partager ou exporter les enregistrements via la feuille de partage iOS, sous votre contrôle
- Les enregistrements ne sont jamais téléversés vers CONEX ou un quelconque tiers par l'Application

Il vous appartient de vous assurer que tout enregistrement ou toute surveillance en direct que vous effectuez est conforme à l'ensemble des lois applicables — y compris aux exigences de consentement qui peuvent s'appliquer là où vous vous trouvez. Voir nos [Conditions d'utilisation](/fr/terms/) et la page [Assistance](/fr/support/) pour en savoir plus.

---

## 7. Tiers, paiements et App Store

- CONEX ne **partage** aucune donnée avec un quelconque tiers.
- L'Application n'utilise **aucun** SDK publicitaire, analytique ou de profilage.
- CONEX ne **vend** ni ne **loue** aucune donnée, quelle qu'elle soit.

La distribution et les paiements sont gérés par Apple via l'App Store et l'Achat intégré (In-App Purchase). **HearRelay Full Access est un achat unique non consommable, et non un abonnement à renouvellement automatique.** Les prix, taxes, remboursements et facturation sont traités par Apple selon les conditions de l'App Store et des Apple Media Services. CONEX ne reçoit ni numéros de carte de paiement ni informations de facturation. Vous pouvez restaurer un achat antérieur via l'option **Restore Purchases** dans l'Application.

Lorsque Apple traite votre achat ou livre des mises à jour, la politique de confidentialité d'Apple s'applique à cette activité. Toute information de diagnostic qu'Apple collecte depuis votre appareil (par exemple les rapports de plantage envoyés via « Partager avec les développeurs d'apps ») est régie par vos Réglages iOS et les conditions développeur d'Apple.

---

## 8. Notre site Web

Le site Web HearRelay à l'adresse <https://hearrelay.app/> est un site informationnel statique hébergé sur GitHub Pages. Nous n'utilisons **aucun** cookie publicitaire, cookie d'analytique, pixel de suivi ni balise marketing tierce. Si cela devait changer, nous mettrions à jour la présente Politique et fournirions toute notification ou option de choix exigée par le droit applicable.

---

## 9. Utilisateurs internationaux

Étant donné que HearRelay ne transfère aucune donnée hors de vos appareils vers les serveurs de CONEX, aucun transfert international de données personnelles n'est effectué par CONEX.

### 9.1 Utilisateurs dans l'Espace économique européen (EEE), au Royaume-Uni et en Suisse

L'Application est conçue de telle sorte que CONEX ne collecte ni ne reçoit sur ses propres serveurs aucun son, enregistrement, information de paiement, donnée analytique, identifiant publicitaire ou donnée de suivi.

Des informations limitées de découverte d'appareils peuvent être stockées dans Apple iCloud, dans le cadre de votre compte Apple ID (§4). CONEX n'exploite pas Apple iCloud et n'accède pas à ces informations sur ses propres serveurs. Lorsque le droit applicable considère ces informations comme des données personnelles, les **finalités** de tout traitement de ce type se limitent à permettre la découverte d'appareils, l'authentification mutuelle, la sécurité et la communication pair à pair locale entre vos propres appareils ; la **base légale** est votre consentement à l'utilisation de l'Application à cette fin, ainsi que votre intérêt légitime à connecter vos propres appareils de manière privée.

CONEX a évalué l'obligation, au titre de l'article 27 du RGPD, de désigner un représentant dans l'Union et a conclu que la nature limitée, occasionnelle et à faible risque de tout traitement entre dans l'exemption prévue à l'article 27(2)(a). Cette évaluation est documentée en interne et fait l'objet d'un réexamen lorsque des éléments substantiels évoluent. Si vous êtes une autorité de contrôle ou une personne concernée dans l'EEE souhaitant nous contacter, veuillez utiliser **hearrelay-privacy@conex-cp.com** — nous nous engageons à répondre dans les délais légaux.

### 9.2 Utilisateurs au Brésil

La posture de traitement de l'Application au regard de la LGPD reflète celle décrite au §9.1. CONEX n'a pas connaissance de données personnelles traitées sur ses propres serveurs. CONEX n'a pas désigné d'Encarregado local (DPO) au motif qu'aucun traitement de données personnelles à grande échelle ou à haut risque n'est effectué par CONEX. Le contact ci-dessus sert de point de contact pour les demandes au titre de la LGPD.

### 9.3 Utilisateurs au Japon

CONEX n'inclut dans l'Application aucun SDK publicitaire, analytique ou de suivi tiers, et ne transmet aucune information relative aux utilisateurs vers ses propres serveurs. Apple iCloud Key-Value Storage est utilisé uniquement pour synchroniser les informations limitées de découverte d'appareils décrites au §4 au sein de votre propre compte Apple ID ; CONEX ne reçoit pas ces informations sur ses propres serveurs. Nous nous référons à cette configuration de bonne foi pour évaluer le régime japonais de notification de transmission externe au titre du Telecommunications Business Act.

### 9.4 Utilisateurs à Hong Kong / Taïwan

La même posture de traitement s'applique. CONEX a conscience que la PDPO (Hong Kong) et la Personal Information Protection Act (Taïwan) définissent largement les notions de données personnelles et d'informations personnelles ; veuillez vous référer aux §4 et §10 pour notre position et les droits que vous pouvez exercer.

---

## 10. Confidentialité des enfants

HearRelay est un utilitaire destiné aux adultes, généralement les parents ou les personnes assurant la garde d'enfants. Il n'est **pas destiné aux enfants de moins de 13 ans**, et CONEX ne collecte pas sciemment de données personnelles concernant des enfants. Le traitement de l'Application est local à votre appareil ; aucune donnée personnelle d'enfant n'est donc collectée, stockée ou transmise à CONEX.

---

## 11. Vos droits

Étant donné que CONEX ne détient aucune donnée personnelle vous concernant sur ses serveurs, il n'y a généralement rien à consulter, rectifier, supprimer, exporter ou limiter. Néanmoins, selon votre localisation (EEE, Royaume-Uni, Californie, Brésil, Japon, Hong Kong, Taïwan, etc.), vous pouvez disposer de droits légaux, notamment :

- Droit d'accès
- Droit de rectification
- Droit à l'effacement
- Droit d'opposition ou de limitation du traitement
- Droit à la portabilité des données
- Droit de refuser la « vente » ou le « partage » — CONEX ne vend ni ne partage de données personnelles
- Droit d'introduire une réclamation auprès de votre autorité de contrôle locale

Pour exercer un droit, contactez **hearrelay-privacy@conex-cp.com**. Veuillez noter que pour supprimer toutes les données stockées localement par l'Application, il vous suffit de désinstaller l'Application de votre appareil. Pour purger l'identité de l'Application propre à votre appareil dans Apple iCloud (§4), utilisez **Réglages → Sécurité → Réinitialiser toute la sécurité de l'appareil** dans l'Application.

---

## 12. Sécurité

Nous utilisons des protections conformes aux standards du secteur :

- **HearRelay Secure Channel** (X25519 ECDH + AEAD ChaCha20-Poly1305) pour toutes les communications d'appareil à appareil
- Clés d'identité **P-256** générées et stockées dans le **Secure Enclave** lorsque celui-ci est pris en charge, avec un repli sur le Keychain
- **Épinglage de clé publique** au moyen d'une liste de confiance dans le périmètre iCloud, afin d'empêcher tout appareil usurpateur de se connecter
- **Protection de fichier** (`NSFileProtectionComplete`) pour les enregistrements locaux

Aucune méthode de transmission ou de stockage n'est parfaitement sécurisée. Pour signaler une vulnérabilité, veuillez consulter notre [page Sécurité](/fr/security/) et écrire à **hearrelay-security@conex-cp.com**.

---

## 13. Modifications de la présente politique

Nous pouvons réviser la présente Politique de confidentialité. La date de révision sera mise à jour en haut de cette page, et les modifications substantielles seront annoncées dans les notes de version de l'Application. Lorsque le droit applicable l'exige, nous obtiendrons votre consentement ou vous fournirons un préavis raisonnable et une véritable possibilité de cesser d'utiliser l'Application avant que la modification ne prenne effet.

---

## 14. Contact

- Confidentialité : **hearrelay-privacy@conex-cp.com**
- Assistance : **hearrelay-support@conex-cp.com**
- Sécurité : **hearrelay-security@conex-cp.com**
- Web : <https://hearrelay.app/>

---

**Traductions disponibles :** [日本語](/ja/privacy/) · [Français](/fr/privacy/) · [Español](/es/privacy/) · [Português (Brasil)](/pt-BR/privacy/) · [简体中文](/zh-Hans/privacy/)

Lorsque la présente Politique est fournie dans une langue autre que l'anglais, la **version anglaise prévaut** dans la mesure permise par le droit applicable. Cette règle de préséance ne limite pas les droits que vous accordent les lois impératives de protection des consommateurs, de la vie privée ou des données de votre pays ou région.
