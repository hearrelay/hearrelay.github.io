---
title: Politique de confidentialité — HearRelay
lang: fr
---

# Politique de confidentialité

**Date d'entrée en vigueur : 24 avril 2026**
**Dernière mise à jour : 24 avril 2026**

> Cette traduction est fournie à titre de commodité. En cas de divergence entre la présente traduction et la [version anglaise](/en/privacy/), la version anglaise prévaut.

HearRelay (« l'Application ») est conçue pour respecter la vie privée par défaut. La présente politique explique quelles données sont, et ne sont pas, traitées lorsque vous utilisez HearRelay.

Pour toute question, veuillez nous contacter à l'adresse **hearrelay-privacy@conex-cp.com**.

---

## 1. Qui nous sommes

HearRelay est développée par **CONEX Corporation** (株式会社CONEX), une société constituée au Japon (« l'Éditeur », « nous »). HearRelay ne traitant aucune donnée personnelle sur nos serveurs, nous ne jouons pas le rôle de « responsable du traitement » au sens substantiel — nous sommes l'éditeur de l'application. Pour tout échange, merci d'utiliser les adresses e-mail en bas de cette page.

---

## 2. Données que nous ne collectons pas

Nous ne collectons, ne stockons, ne transmettons à nos serveurs et ne partageons **aucune** des données suivantes :

- Les sons captés par le microphone de votre appareil
- Les enregistrements audio que vous créez avec l'Application
- Coordonnées, localisation, photos, images caméra ou identifiants d'appareil
- Identifiants publicitaires (IDFA, IDFV utilisé à des fins de suivi)
- Analyses, télémétrie de plantage envoyée à des services tiers, profils comportementaux

HearRelay ne contient aucun SDK tiers d'analytique, de publicité ou de suivi.

---

## 3. Données traitées localement sur votre appareil

L'Application traite les éléments suivants sur votre appareil, et **uniquement sur votre appareil** :

| Donnée | Finalité | Conservation |
|---|---|---|
| Audio du microphone (temps réel) | Écoute en temps réel via un casque ou un appareil apparié sur le même Wi-Fi | Non stockée |
| Enregistrements audio (optionnel) | Vous pouvez enregistrer des sessions manuellement | Supprimés automatiquement après 24 heures par défaut ; vous pouvez prolonger ou supprimer plus tôt |
| Historique de connexion (nom du pair, dernière connexion) | Fonction de commodité pour se reconnecter rapidement | Stocké localement ; effacé lors de la désinstallation |
| Préférences de l'application | Mémoriser vos réglages | Stockées localement |

Lorsque vous désinstallez l'Application, toutes ces données sont supprimées.

---

## 4. Données transitant brièvement par l'infrastructure Apple

Afin de permettre à vos propres appareils Apple de se découvrir sur le même Wi-Fi, HearRelay utilise **iCloud Key-Value Storage**, fourni par Apple, pour publier :

- Une **clé publique** cryptographique générée sur votre appareil
- Une **empreinte** (SHA-256) de cette clé
- Le **nom** de l'appareil, sa **plateforme**, son **modèle** et la **version de l'application**

Ces données sont stockées dans la portée de votre propre identifiant Apple, au sein du service iCloud d'Apple, et ne sont pas visibles par d'autres titulaires d'identifiants Apple ni par nous. L'Éditeur n'exploite aucun serveur et n'a pas accès à ces données. Le traitement par Apple est régi par la politique de confidentialité d'Apple.

---

## 5. Communications réseau

HearRelay communique **uniquement** avec d'autres appareils Apple qui :

1. Sont connectés au **même identifiant Apple**, **et**
2. Sont sur le **même Wi-Fi / réseau local**

Les communications sont chiffrées avec **TLS 1.3**. HearRelay n'envoie **aucune** donnée via Internet vers des serveurs distants et ne prend pas en charge la surveillance à distance entre réseaux. L'usage distant est délibérément interdit pour prévenir toute surveillance dissimulée.

---

## 6. Enregistrements que vous créez

Si vous activez la fonction d'enregistrement :

- Les enregistrements sont sauvegardés **uniquement sur l'appareil qui les a créés**
- Ils sont stockés dans le bac à sable de l'Application avec un **chiffrement au niveau fichier** (`NSFileProtectionComplete`)
- Ils sont **automatiquement supprimés 24 heures** après leur création, sauf si vous décidez explicitement de les conserver
- Vous pouvez les partager ou les exporter via la feuille de partage iOS, sous votre contrôle
- Les enregistrements ne sont jamais téléversés vers nous ou vers un tiers par l'Application

---

## 7. Tiers

- Nous ne partageons **aucune** donnée avec un tiers.
- Nous n'utilisons **aucun** SDK publicitaire, d'analytique ou de profilage.
- Nous ne vendons ni ne louons aucune donnée.

La distribution et le paiement sont gérés par Apple via l'App Store selon les conditions d'Apple. Lorsque Apple traite votre achat ou livre des mises à jour, la politique de confidentialité d'Apple s'applique à cette activité.

---

## 8. Utilisateurs internationaux

HearRelay ne transférant aucune donnée en dehors de vos appareils, aucun transfert international de données personnelles n'est effectué par nous.

---

## 9. Confidentialité des enfants

HearRelay est un utilitaire destiné aux adultes, généralement les parents ou les personnes assurant la garde d'enfants. Il **ne s'adresse pas aux enfants de moins de 13 ans** et nous ne collectons pas sciemment de données personnelles concernant les enfants. Le traitement de l'Application se déroule localement sur votre appareil, aucune donnée personnelle d'enfant n'est donc collectée, stockée ou transmise.

---

## 10. Vos droits

Nous ne détenant aucune donnée personnelle à votre sujet, il n'y a généralement rien à consulter, rectifier, supprimer, exporter ou limiter. Néanmoins, selon votre localisation (EEE, Royaume-Uni, Californie, Brésil, Japon, etc.), vous pouvez bénéficier de droits légaux, notamment :

- Droit d'accès
- Droit de rectification
- Droit à l'effacement
- Droit d'opposition ou de limitation du traitement
- Droit à la portabilité des données
- Droit d'introduire une réclamation auprès de votre autorité locale de contrôle

Pour exercer l'un de ces droits, contactez-nous à **hearrelay-privacy@conex-cp.com**. Pour supprimer toutes les données stockées localement par l'Application, il vous suffit de désinstaller l'Application de votre appareil.

---

## 11. Sécurité

Nous utilisons des protections de niveau industriel :

- **TLS 1.3** pour toutes les communications d'appareil à appareil
- Clés **Curve25519 / P-256** générées et stockées dans le **Secure Enclave** lorsque l'appareil le permet
- **Épinglage de clé publique** pour empêcher toute connexion par un appareil usurpateur
- **Protection de fichier** (`NSFileProtectionComplete`) pour les enregistrements locaux

Aucune méthode de transmission ou de stockage n'est parfaitement sécurisée. Pour signaler une vulnérabilité, consultez notre [page de sécurité](/fr/security/) et écrivez à **hearrelay-security@conex-cp.com**.

---

## 12. Modifications de la présente politique

Nous pouvons réviser la présente politique de confidentialité. La date de révision sera mise à jour en haut de cette page, et les changements importants seront annoncés dans les notes de version de l'Application. La poursuite de l'utilisation de l'Application après l'entrée en vigueur des modifications vaut acceptation.

---

## 13. Contact

- Confidentialité : **hearrelay-privacy@conex-cp.com**
- Assistance : **hearrelay-support@conex-cp.com**
- Sécurité : **hearrelay-security@conex-cp.com**
- Web : <https://hearrelay.github.io/>

---

**English version:** [Privacy Policy](/en/privacy/)
