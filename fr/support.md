---
title: Assistance — HearRelay
lang: fr
---

> La présente version française est fournie à titre de commodité. En cas de divergence ou d'incohérence entre cette version et la version anglaise, la version anglaise prévaut dans la mesure permise par le droit applicable. Cette règle de préséance ne limite pas les droits que vous accorde le droit impératif en matière de protection des consommateurs, de la vie privée ou des données.

# Assistance

**Version du document : v3.2026-04-26**

Merci d'utiliser **HearRelay**. Cette page rassemble des conseils de dépannage, des avertissements importants concernant un usage licite, et nos coordonnées.

---

## Avertissements importants

### Les lois sur l'enregistrement et la surveillance varient selon les lieux

Les lois relatives à l'enregistrement et à la surveillance en direct varient selon le pays, l'État, la province et le lieu d'utilisation. Certains lieux exigent le consentement de **toutes** les parties avant tout enregistrement. La surveillance dans un lieu de travail, une école, une location, un cadre médical, de soin aux personnes âgées, de garde d'enfants ou un espace public peut nécessiter une notification spécifique, un consentement écrit ou une autorisation. **N'enregistrez pas de conversations ni d'espaces privés à moins d'y être légalement autorisé.** En cas de doute, n'enregistrez pas.

Il vous appartient de vous assurer que tout enregistrement ou toute surveillance en direct que vous effectuez avec HearRelay est conforme à l'ensemble du droit applicable. Voir la liste des usages interdits aux [Conditions d'utilisation §3](/fr/terms/).

### HearRelay n'est pas un dispositif de sécurité, médical ou d'urgence

HearRelay est un utilitaire grand public destiné à une surveillance de commodité. Ce n'est **pas** un dispositif médical, un dispositif d'urgence, une alarme de sécurité, un dispositif de sécurité pour enfants, un dispositif de sécurité pour personnes âgées, un dispositif de maintien des fonctions vitales, ni un équipement certifié pour un usage critique de sécurité. **N'utilisez jamais HearRelay comme moyen unique de surveillance ou de détection d'urgence.** Combinez-le toujours avec une surveillance directe responsable et tout équipement de sécurité certifié à cet effet.

### Pourquoi HearRelay ne fonctionne pas par Internet

HearRelay exige délibérément que les deux appareils soient **connectés au même Apple ID** *et* **connectés au même Wi-Fi / réseau local**. Il n'existe aucune option de relais via Internet, aucun mode de surveillance à distance et aucune voie « cloud ». Il s'agit d'un choix de sécurité et de confidentialité, et non d'une fonctionnalité manquante :

- Cela empêche toute surveillance à distance dissimulée — un iPhone volé ou emprunté ne peut pas diffuser l'audio hors du domicile de quelqu'un.
- Cela maintient l'audio hors des serveurs CONEX (nous n'en exploitons aucun) et hors de l'Internet public.
- Cela limite l'impact d'une compromission de l'Apple ID aux appareils déjà appariés à cet Apple ID.

Si vous avez besoin d'une surveillance entre réseaux, HearRelay n'est pas l'outil approprié — utilisez un produit certifié à cet effet, avec la notification parentale, professionnelle ou autre légalement requise.

---

## Aide rapide

### « Aucun appareil trouvé » lors de l'appairage

Les deux appareils doivent :

1. Être connectés au **même Apple ID**
2. Être connectés au **même réseau Wi-Fi** (même sous-réseau)
3. Avoir **iCloud** activé dans les Réglages iOS
4. Avoir accordé à HearRelay les autorisations **Microphone** et **Réseau local**

Si vous ne voyez toujours pas l'autre appareil, appuyez sur le bouton d'actualisation du sélecteur d'appairage, ou redémarrez l'Application sur les deux appareils.

### Le son saute ou se coupe

- Rapprochez-vous de votre routeur Wi-Fi ou passez à un réseau 5 GHz
- Des écouteurs Bluetooth à faible réception peuvent introduire des coupures — essayez un modèle filaire ou un autre modèle
- Un trafic réseau intense (téléchargements volumineux, visioconférences) sur le même Wi-Fi peut affecter l'audio en temps réel

### Le son provenant des AirPods est étrangement de mauvaise qualité en mode Standalone

HearRelay restreint le microphone au **micro intégré** en mode Standalone afin d'éviter de forcer le Bluetooth dans un mode à faible bande passante (HFP). Utilisez le micro intégré en entrée et les AirPods uniquement en sortie. Cela est voulu.

### Mon enregistrement n'est plus là

Les enregistrements sont automatiquement supprimés **24 heures après leur création** sauf si vous appuyez sur **Conserver** sur l'enregistrement. Une fois conservés, ils restent jusqu'à ce que vous les supprimiez.

### HearRelay a cessé d'enregistrer lorsque j'ai verrouillé l'écran

HearRelay continue de capturer et de retransmettre l'audio en arrière-plan lorsque l'écran est verrouillé. Si la capture s'arrête :

- Vérifiez que **Background App Refresh** est autorisé pour HearRelay (Réglages iOS → Général → Background App Refresh)
- Vérifiez que le **mode économie d'énergie** ne suspend pas agressivement les tâches en arrière-plan
- Certaines versions d'iOS suspendent les sessions audio lorsqu'une autre application audio prend le relais — arrêtez cette autre application

### L'icône dans Dynamic Island / l'écran verrouillé a disparu

Les Live Activities ont une durée maximale imposée par l'OS (environ 8 heures). Une fois cette durée atteinte, l'indicateur peut cesser de se mettre à jour même si HearRelay continue de fonctionner. Rouvrez l'Application pour rafraîchir.

**Important :** Même si une Live Activity ou un widget de l'écran verrouillé cesse de se mettre à jour en raison des limites de l'OS, **la capture audio en arrière-plan peut se poursuivre tant que la surveillance est active**. N'utilisez ceci que dans des situations de surveillance licites et divulguées. Ne placez pas un appareil là où il pourrait capter des personnes n'ayant pas reçu la notification ou le consentement légalement requis. iOS peut également afficher ses indicateurs système de microphone / confidentialité pendant que la capture audio est active.

---

## Achats et abonnements

### HearRelay est-il un abonnement ?

**Non.** HearRelay Full Access est un **achat unique non consommable** (un IAP de type achat ferme). Ce n'est **pas** un abonnement à renouvellement automatique. Après la période d'essai gratuite de 14 jours, un achat unique débloque l'Application aussi longtemps que vous restez connecté à votre Apple ID.

### Family Sharing

Le déverrouillage est activé pour **Family Sharing**, ce qui permet aux membres de votre groupe Family Sharing d'utiliser HearRelay Full Access sans coût supplémentaire.

### Comment restaurer un achat antérieur ?

Ouvrez l'Application → appuyez sur la bannière verrouillée → **Restore Purchases**. Apple vérifiera dans votre Apple ID le déverrouillage antérieur et le réappliquera.

### Comment obtenir un remboursement ?

Les demandes de remboursement pour les achats effectués sur l'App Store doivent être soumises via le processus de remboursement standard d'Apple à l'adresse <https://reportaproblem.apple.com>. Apple traite les remboursements selon les conditions de l'App Store et des Apple Media Services. CONEX ne reçoit ni numéros de carte de paiement ni informations de facturation. Rien dans le présent paragraphe ne limite les droits impératifs de consommateur dont vous pourriez disposer à l'encontre de CONEX au titre du droit applicable.

---

## Liste de vérification des autorisations

| Autorisation | Nécessaire pour | Chemin des réglages |
|---|---|---|
| Microphone | Toute surveillance | Réglages → HearRelay → Microphone |
| Réseau local | Mode appairé (envoi / réception avec d'autres appareils) | Réglages → HearRelay → Réseau local |
| iCloud (connecté) | Mode appairé (découvrir vos autres appareils) | Réglages → \[Votre nom\] → iCloud |
| Background App Refresh | Surveillance continue avec l'écran éteint | Réglages → Général → Background App Refresh |

Si le réseau local ou iCloud n'est pas disponible, vous pouvez toujours utiliser le mode **Standalone**.

---

## Contact

- **E-mail :** hearrelay-support@conex-cp.com
- Nous visons à répondre sous quelques jours ouvrés. Merci de préciser votre version d'iOS, le modèle d'appareil et une description des étapes effectuées.

Pour les questions de confidentialité, voir la [Politique de confidentialité](/fr/privacy/) ou écrire à **hearrelay-privacy@conex-cp.com**.
Pour les signalements de sécurité, voir la [page Sécurité](/fr/security/) ou écrire à **hearrelay-security@conex-cp.com**.

---

**Traductions disponibles :** [日本語](/ja/support/) · [Français](/fr/support/) · [Español](/es/support/) · [Português (Brasil)](/pt-BR/support/) · [简体中文](/zh-Hans/support/)

Lorsque la présente page est fournie dans une langue autre que l'anglais, la **version anglaise prévaut** dans la mesure permise par le droit applicable. Cette règle de préséance ne limite pas les droits que vous accordent les lois impératives de protection des consommateurs, de la vie privée ou des données de votre pays ou région.
