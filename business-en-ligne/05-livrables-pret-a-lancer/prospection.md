# SOP Prospection J2 (et routine quotidienne)

**Objectif J2** : constituer une liste de **30–50 cibles FR** qualifiées et avoir le **1er message prêt**.
**Niches par défaut** (alignées sur les démos) : **coiffeurs à Lyon** et **plombiers à Bordeaux**. À adapter en 1 min en remplaçant les mots-clés.

> ⚠️ Les lignes `EXEMPLE_` du fichier `cibles.csv` sont des gabarits. Remplacez-les par de **vraies** entreprises issues de Google Maps (voir méthode ci-dessous). N'envoyez jamais à des faux contacts.

---

## 1. Construire la liste en 30 min (Google Maps)
1. Ouvrez Google Maps, cherchez `coiffeur Lyon` (puis `plombier Bordeaux`).
2. Cliquez les résultats un par un : those **sans site web** ou avec un site **obsolète/lent** = cibles prioritaires.
3. Pour chacun, notez : nom, ville, présence site (oui/non/obsolète), moyen de contact (fiche Maps / Messenger / email / tel), canal.
4. Collez dans `cibles.csv`. Visez 30–50 lignes réelles.
5. Complétez avec des groupes Facebook « Commerçants [ville] » et LinkedIn (recherche métier + ville).

## 2. Routine quotidienne (≤ 2 h, du J4 au J30)
- **30 min** : 10 nouveaux contacts qualifiés (Maps / groupes / LinkedIn) → ajout au CSV.
- **15 min** : relances J+3 et J+7 des contacts précédents.
- **75 min** : production si commande en cours (construction/modif site).
- **5 min** : mise à jour du suivi (`suivi-quotidien.md` ou CSV).

## 3. Message n°1 (Script A) — Coiffeuse à Lyon
```
Bonjour {{PRENOM}},
Je suis tombé sur votre fiche et je vois que vous n'avez pas encore de site web.
Sans juger : est-ce que vous aimeriez apparaître quand on cherche "coiffeuse Lyon" sur Google ?
Je crée des sites pros clés en main en 5 jours (dès 190 € HT, sans engagement, paiement à la livraison).
Je peux vous faire un audit gratuit de 5 min si ça vous dit.
```
## 3b. Message n°1 (Script A) — Plombier à Bordeaux
```
Bonjour {{PRENOM}},
Petite question pratique : quand un client cherche "plombier Bordeaux" sur son téléphone, est-ce qu'il vous trouve ?
Je crée des sites vitrines pros, livrés en 5 jours, dès 190 € HT, sans abonnement.
Je peux vous envoyer un exemple conçu pour un plombier, ça vous dit ?
```

## 4. Relances
- **J+3** : « Bonjour {{PRENOM}}, je me permets de revenir : mon offre de site clé en main (5 jours, dès 190 € HT) tient toujours. Je peux vous préparer un devis personnalisé sous 24 h ? »
- **J+7** : « Dernier message de ma part : si le moment est mal choisi, pas de souci. Au plaisir si besoin un jour. »

## 5. Dès une réponse intéressée → devis
Utilisez `devis-template.html` (remplir les {{...}}), envoyez-le, et à validation : **acompte 50 % via Payoneer Payment Request**.

---

## PRÉPARATION TEST J3 (obligatoire avant prospection à grande échelle)
Le but : valider la chaîne **Payoneer → MCB** avec un vrai micro-paiement.
1. Dans Payoneer → « Receive » → « Payment Request » → créez une demande de **2–5 €** à un proche français.
2. Le proche paie par **virement SEPA** vers votre compte de réception EUR Payoneer (frais réception ~1 %) — ou par carte (jusqu'à 3,99 %).
3. Une fois reçu, lancez le **retrait vers MCB** (frais ~1,2–4 %).
4. Confirmez l'arrivée sur la carte MCB et notez les **frais réels** dans `journal.md`.
→ Si l'argent arrive : la chaîne est validée, vous pouvez prospecter sereinement. Sinon, résolvez (virement SWIFT direct MCB possible en repli) avant de poursuivre.

## Indicateurs visés (cumul J30)
≥ 200 contacts · ≥ 20 réponses · ≥ 6 devis · ≥ 3 ventes · 400–1 200 € nets MCB · **0 € dépensé**.
