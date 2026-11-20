# 01 — Vérification des faits : encaisser depuis Madagascar des clients français/européens

**Méthode** : recherche web du 2026-11-20. Chaque affirmation est sourcée (URL + date). Où l'information est absente ou contradictoire, j'écris **NON VÉRIFIÉ**.

---

## 0. VERDICT RAPIDE (à lire en premier)

Pour un résident malgache qui veut vendre à la France/Europe et faire atterrir l'argent sur sa **carte MCB Banque (Madagascar)**, voici la réalité vérifiée :

| Chaîne | Réception en MG ? | Encaissement vers MCB | Verdict |
|---|---|---|---|
| **Payoneer** (hub central) | OUI (Madagascar accepté) | OUI, retrait vers compte bancaire local (MCB) en 2-5 j | ✅ **Chaîne principale recommandée** |
| **Paddle** (Merchant of Record) | OUI (Madagascar dans les pays vendeurs) | OUI, virement SWIFT mensuel vers MCB | ✅ Pour produits numériques/soft |
| **Virement SWIFT direct client → MCB** | OUI (MCB a un code SWIFT) | OUI | ✅ Pour B2B avec facture |
| **Digistore24** (via Payoneer) | OUI | Via Payoneer → MCB | ✅ Repli affiliation/produit |
| **Fiverr / Upwork** (via Payoneer) | OUI | Via Payoneer → MCB | ✅ Pour services freelance |
| **PayPal** | ❌ **Réception impossible en MG** | ❌ Retrait vers banque locale impossible | 🚫 **À ÉVITER** |
| **Stripe** (compte vendeur direct) | ❌ MG non supporté comme vendeur | N/A | 🚫 Non dispo pour toi |
| **Payhip / Gumroad** | ⚠️ Paient via PayPal/Stripe → bloqués en MG | ❌ | 🚫 Risqué en l'état |
| **Lemon Squeezy** | OUI payout MG… mais arrêt prévu 31/03/2027 | N/A | ⚠️ Risqué pour nouveau vendeur |
| **Wise** | Réception EUR/USD OK, mais **pas d'envoi MGA vers MG** | ❌ "last mile" bloqué | ⚠️ Secondaire |

**Conclusion opérationnelle** : La chaîne la plus sûre et 100 % vérifiée est **Payoneer comme hub** (clients et marketplaces y envoient l'argent, tu retires vers MCB), complétée par **Paddle** pour les produits numériques (car Paddle gère la TVA à ta place = Merchant of Record). PayPal est à bannir pour l'encaissement Madagascar.

---

## 1. Détail par plateforme (faits + sources)

### 1.1 PayPal — ❌ Réception et retrait IMPOSSIBLES à Madagascar
- Les fonctionnalités de **réception et de retrait vers un compte bancaire local ne sont pas disponibles** à Madagascar. On peut payer en ligne, mais pas encaisser.
- Source officielle (community PayPal) : *"Je vous confirme qu'il n'est pas encore possible d'y recevoir des paiements"* — https://www.paypal-community.com/t5/Vos-remarques-et-suggestions/Compte-en-ligne-car-recevoir-de-l-argent-%C3%A0-Madagascar-est/m-p/1534604
- Presse locale (L'Express Madagascar, 28/05/2026) : *"les retraits directs vers un compte bancaire local ne sont pas encore disponibles"* — https://www.lexpress.mg/2026/05/technologie-paypal-elargit-lacces-en.html
- Frais si compte ailleurs (hors sujet ici) : réception internationale 4,90 % +固定 (MG dans la liste) — https://www.paypal.com/mg/business/paypal-business-fees
- **Conséquence** : ne propose PAS PayPal comme moyen de paiement à tes clients français. Contournements type PRIPEO (PayPal → Mobile Money, délai 5 j, frais par transaction) existent mais restent fragiles — https://pripeo.com/paypal-madagascar-recevoir-retirer-argent/

### 1.2 Payoneer — ✅ Disponible à Madagascar, retrait vers banque locale possible
- Madagascar figure dans la liste des **212 pays acceptés** — https://worldpopulationreview.com/country-rankings/payoneer-countries ; https://help.smartcat.com/payoneer/
- **Comptes de réception locaux** (USD, EUR, GBP…) : le client paie comme un local (virement, carte, ACH). — https://www.payoneer.com/get-paid-by-clients/
- **Payment Request** : tu émets une facture, le client paie par carte / virement / PayPal / débit bancaire direct ; l'argent arrive sur ton compte Payoneer. — https://www.payoneer.com/resources/how-to-use-payoneer/how-to-use-payoneer-guide/
- **Marketplaces** : Fiverr, Upwork, Amazon, Airbnb… versent directement sur Payoneer. — https://www.payoneer.com/freelancer/
- **Retrait vers banque locale** : 2 à 5 jours ouvrés. Frais : 1,50 $ si retrait dans la même devise/pays ; sinon **1,2 % à 4 %** (conversion incluse, milieu ~2,6 %). — https://feebite.com/blog/payoneer-fees-explained ; https://www.fastlancer.org/en/fastlancer-blog/payoneer-review/ ; https://dodopayments.com/blogs/payoneer-fees-explained
- Payoneer facture **29,95 $/an** si tu reçois moins de 6 000 $ sur 12 mois (sinon gratuit pour le compte).
- **Carte prépayée Mastercard** disponible pour dépenser/retirer au distributeur (utile, mais le retrait vers MCB reste la cible).

### 1.3 Wise — ⚠️ Réception OK, mais "last mile" vers MGA bloqué
- Un résident malgache **peut ouvrir un compte et recevoir EUR/USD/GBP** avec des coordonnées locales (IBAN européen, etc.) — https://wise.com/help/articles/2897238/which-currencies-can-i-add-keep-and-receive-in-my-wise-account
- MAIS **Wise ne permet pas d'envoyer des MGA vers un compte bancaire malgache** ; Madagascar n'est pas une devise de réception. — https://voyagiste-madagascar.com/wise-and-revolut-in-madagascar-do-they-work-2026-guide/
- Certaines banques malgaches (BFV-SG, BMOI) détiendraient des comptes USD/EUR (à vérifier pour MCB — **NON VÉRIFIÉ** pour MCB).
- **Usage** : peut servir de "réceptacle" EUR si un jour tu as un compte bancaire étranger ; pas une solution directe vers MCB aujourd'hui.

### 1.4 Stripe — ❌ Pas de compte vendeur à Madagascar
- Stripe ne permet **pas** à un résident de Madagascar d'ouvrir un compte vendeur direct (MG n'est pas dans les ~46 pays supportés). — https://get.bandcamp.help/hc/en-us/articles/32854280223511-Which-countries-are-supported-by-Stripe-payments
- Stripe a ajouté Madagascar comme **pays de paiement sortant** (Global Payouts, MGA) — https://docs.stripe.com/global-payouts/recipient-countries — mais c'est pour les plateformes qui payent des bénéficiaires, pas pour que TU sois le marchand Stripe.
- **Conséquence** : pas de Stripe Checkout pour toi. (Les outils qui dépendent de Stripe pour payer le vendeur — Payhip, Gumroad partiellement — en souffrent en MG.)

### 1.5 Paddle (Merchant of Record) — ✅ Pour produits numériques/software, paie Madagascar
- Madagascar figure dans les **pays vendeurs supportés** (228 "Yes"). — https://getpaidatlas.com/provider/paddle ; https://developer.paddle.com/concepts/sell/supported-countries-locales.md
- **Paddle est le vendeur de record** : il collecte et reverse la TVA dans 100+ juridictions. Tu ne t'occupes PAS de la TVA. — https://www.paddle.com/help ; https://finzil.com/providers/paddle
- **Paiement** : mensuel (seuil min 100 $), par virement ou Payoneer. Virement SWIFT = 15 $ si la devise diffère du pays de la banque ; conversion jusqu'à 1,5 %. — https://www.paddle.com/help/manage/get-paid ; https://agentaos.ai/answers/paddle-fees
- Frais par vente : **5 % + 0,50 $**. — https://finzil.com/providers/paddle
- **Limite** : Paddle est réservé au **software / SaaS / produits numériques**. Il **interdit les services** (contrairement à Lemon Squeezy qui les interdisait aussi). Donc Paddle = pour vendre un produit numérique (template, kit, outil, formation en ligne), pas pour facturer une prestation humaine.

### 1.6 Lemon Squeezy — ⚠️ Payout MG oui, mais arrêt prévu le 31/03/2027
- Madagascar est dans les ~119 pays de paiement bancaire. — https://www.flowclique.com/2026/10/lemon-squeezy-supported-countries.html
- MAIS Lemon Squeezy **arrête le paiement le 31/03/2027** et migre vers "Stripe Managed Payments" qui ne couvre que 37 pays (Madagascar exclu). Pour un nouveau vendeur, c'est un cul-de-sac. — https://www.merchantofrecordfinder.com/blog/lemon-squeezy-shutting-down (17/11/2026)
- **Recommandation** : ne pas démarrer un nouveau business dessus aujourd'hui.

### 1.7 Gumroad — ⚠️ MoR, mais paiement dépendant de PayPal/Stripe (bloqué en MG)
- MoR depuis janv 2025, gère la TVA. Frais ~10 %. — https://www.shareuhack.com/en/posts/digital-product-platform-comparison-asia-2026
- Paiement aux créateurs : **virement bancaire direct OU PayPal uniquement** ; **pas de Payoneer ni Wise**. — https://grey.co/blog/how-to-receive-payments-from-gumroad-as-an-international-creator ; https://agentaos.ai/answers/gumroad-payout-not-available-in-my-country
- Comme PayPal ne reçoit pas en MG, le paiement Gumroad → toi est **incertain**. 🚫 Risqué.

### 1.8 Payhip — ⚠️ Paie vers TON Stripe/PayPal (donc bloqué en MG)
- Payhip envoie chaque vente **directement vers ton compte Stripe ou PayPal** (pas de solde Payhip). — https://selfmadenewbie.com/payhip-review/ ; https://cartmango.com/payhip-review/
- Comme Stripe n'est pas dispo pour toi et PayPal ne reçoit pas en MG → **Payhip ne peut pas te payer**. 🚫

### 1.9 Digistore24 — ✅ Via Payoneer (repli produit/affiliation)
- Plateforme allemande (depuis 2013), présente dans 100+ pays, gère la TVA UE. Frais ~7,9 % + 1 $. — https://earnifyhub.com/blog/affiliate/digistore24-review-2026 ; https://adplexity.io/blog/affiliate-campaigns-clickbank-buygoods-digistore
- Paiement aux vendeurs/affiliés : **PayPal, virement, Payoneer, Wise, SWIFT**. Le mode "US bank transfer (ACH)" utilise un **compte de réception Payoneer**. — https://help.digistore24.com/hc/en-us/articles/23543008174993-How-to-get-paid-to-your-Payoneer-account
- **Usage** : vendre ton propre produit numérique OU faire de l'affiliation, encaisser via Payoneer → MCB. Bon repli si Paddle refuse ton type de produit.

### 1.10 Print-on-demand (Printful, Gelato, Printify) — ⚠️ L'encaissement reste le goulot
- Pas de coût initial, impression à la commande, expédition par le fournisseur. — https://www.gelato.com/blog/printful-vs-printify ; https://www.atomm.com/blog/2845-print-on-demand-sites
- MAIS ces plateformes **ne te paient pas** : elles impriment ; c'est **toi** qui encaisses via ta caisse (Stripe/PayPal…) sur ta boutique. Donc le même goulot d'encaissement MG. Les marketplaces type Redbubble paient via PayPal (bloqué). 🚫 Complexe pour démarrer à 0 € depuis MG.

### 1.11 Freelance marketplaces (Fiverr, Upwork) — ✅ Via Payoneer
- Les deux versent les gains via **Payoneer** (partenariat historique, 15 ans avec Upwork). — https://www.payoneer.com/freelancer/ ; https://www.fastlancer.org/en/fastlancer-blog/payoneer-review/
- Valable si tu démarres en tant que freelance sur ces plateforms (concurrence forte, mais paiement MG garanti).

### 1.12 MCB Banque (Madagascar) — ✅ Reçoit les virements SWIFT
- **SWIFT/BIC : MCBLMGMGXXX** (The Mauritius Commercial Bank (Madagascar) SA, Antananarivo). — https://www.xe.com/swift-codes/countries/madagascar/mcb-madagascar-swift-code/ ; https://wise.com/gb/swift-codes/MCBLMGMGXXX
- MCB **reçoit des fonds via SWIFT** (délai min 3 jours ouvrés selon la banque correspondante). — https://mcb.mu/corporate/faq/banking
- Donc un virement SWIFT (de Payoneer, de Paddle, ou d'un client) arrive sur ton compte MCB, puis ta carte MCB fonctionne.

---

## 2. Conformité fiscale et légale (vendeur hors UE → clients UE)

### 2.1 TVA sur services numériques B2C vendus à l'UE depuis Madagascar
- Un vendeur **établi hors UE** qui vend des services numériques à des **particuliers (B2C) de l'UE** doit s'enregistrer au régime **OSS Non-UE dès le 1er euro** (pas de seuil pour les non-résidents). Il collecte la TVA au taux du pays du client (ex. 20 % France). — https://experts-tva.com/tva-entreprises-etrangeres/obligations-tva-non-residents/ ; https://support.taxually.com/support/solutions/articles/80001155457-digital-services-vat-in-the-eu-non-union-oss ; https://bofip.impots.gouv.fr/bofip/13240-PGP.html/identifiant=BOI-TVA-DECLA-20-20-60-10-20220629
- **Solution qui t'évite ça** : utiliser un **Merchant of Record** (Paddle, Lemon Squeezy, Gumroad-en-MoR). Lui est le vendeur de record et gère la TVA. Tu ne t'immatricules pas à l'OSS. — https://finzil.com/providers/paddle ; https://www.paddle.com/help
- **Pour les services B2B** (client pro avec n° de TVA intracommunautaire) : **autoliquidation / reverse charge**. Tu factures en HT, le client déclare la TVA chez lui. Pas de TVA à collecter pour toi. — https://www.freebe.me/blog/micro-entrepreneur-vente-a-letranger-obligations-2026 ; https://bofip.impots.gouv.fr

### 2.2 Statut légal minimal pour vendre depuis Madagascar (à confirmer avec un comptable MG)
- **NON VÉRIFIÉ** : les règles exactes pour qu'un résident malgache facture des clients étrangers (en tant que particulier vs entreprise individuelle vs société). À vérifier auprès d'un expert-comptable / guichet unique à Madagascar (ex. registre de commerce, statut d'auto-entrepreneur malgache si existant).
- Ce qui est sûr : tu devras **déclarer ces revenus en Madagascar** (impôt sur le revenu des résidents sur les revenus mondiaux). Barèmes exacts : **NON VÉRIFIÉ** (à confirmer).
- Côté français : pour du **B2B avec reverse charge**, tu n'as pas à t'immatriculer en France tant que tu n'y as pas d'établissement stable. Tu fournis une facture avec ton identité et le n° de TVA du client.

### 2.3 Plateformes qui acceptent des vendeurs malgaches SANS société européenne
- **Payoneer** : compte individuel/freelance accepté (ID requise). — https://www.fastlancer.org/en/fastlancer-blog/payoneer-review/
- **Paddle** : vendeur individuel/entreprise accepté depuis Madagascar. — https://getpaidatlas.com/provider/paddle
- **Digistore24** : vendeur/affilié individuel accepté. — https://help.digistore24.com
- **Fiverr / Upwork** : comptes individuels acceptés, paiement via Payoneer.
- **NON** : Stripe (compte vendeur), Payhip (dépend de Stripe/PayPal MG), Gumroad (PayPal MG).

### 2.4 Autres obligations (RGPD, mentions légales, CGV, rétractation)
- Vente à des consommateurs français/EU → **mentions légales, CGV, politique de confidentialité RGPD, droit de rétractation** obligatoires. Pour les **contenus numériques**, le droit de rétractation peut être **renoncé si le consommateur consent expressément et l'exécution a commencé** (art. L. 221-28 du Code de la consommation) — à préciser clairement dans les CGV.
- Pour du **B2B** (entreprise à entreprise), ces règles de consommation ne s'appliquent pas de la même façon (pas de rétractation de 14 j imposée), mais mentions légales + CGV + facture restent nécessaires.

---

## 3. Tableau synthétique des chaînes de paiement (client → toi → MCB)

| Source du paiement | Outil | Frais approx. | Délai | Arrivée MCB |
|---|---|---|---|---|
| Client pro FR (B2B) | Payoneer Payment Request → retrait MCB | 1,2-4 % (retrait) | 2-5 j | ✅ |
| Client pro FR (B2B) | Virement SWIFT direct → MCB | frais correspondant ~10-40 $ | 3+ j | ✅ |
| Produit numérique | Paddle → virement MCB | 5 %+0,50 $ + 15 $ SWIFT + ≤1,5 % | mensuel | ✅ |
| Affiliation/produit | Digistore24 → Payoneer → MCB | ~7,9 %+1 $ + retrait 1,2-4 % | net-14 | ✅ |
| Freelance | Fiverr/Upwork → Payoneer → MCB | plateforme ~20 % + retrait 1,2-4 % | bi-mensuel | ✅ |
| Client particulier FR (B2C) | PayPal | ❌ impossible en MG | — | 🚫 |

---

## Questions ouvertes / besoins de l'humain
1. **As-tu déjà un compte Payoneer** (ou es-tu prêt à en ouvrir un avec ta pièce d'identité malgache) ? C'est le socle de l'encaissement.
2. **Ton compte MCB est-il en MGA, ou dispose-t-il d'un compte USD/EUR** (pour réduire les frais de conversion) ? À confirmer auprès de MCB.
3. **Statut légal en Madagascar** : es-tu enregistré pour facturer à l'étranger (particulier déclarant, auto-entrepreneur, ou société) ? À valider avec un comptable malgache.
4. **Type d'offre** : services B2B (reverse charge, simple) OU produits numériques B2C (via Paddle, MoR) ? La décision Phase 4 tranche.
