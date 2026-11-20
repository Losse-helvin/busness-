# 00 — Résumé exécutif

**Objectif** : 1 business en ligne, 0 € de budget, cible France puis EU francophone, encaissable sur carte **MCB Banque (Madagascar)**, conforme droit FR/EU, réalisable seul avec l'IA.

**Fait #1 (critique)** : **PayPal ne permet PAS la réception d'argent à Madagascar** (confirmé par PayPal community + presse locale 2026). Interdit comme moyen d'encaissement. Stripe non plus (MG non supporté comme vendeur). Payhip/Gumroad dépendent de PayPal/Stripe → bloqués.

**Fait #2 (solution)** : La chaîne vérifiée est **Payoneer comme hub** (clients + marketplaces → Payoneer → retrait vers MCB, frais 1,2-4 %) et **Paddle** (Merchant of Record) pour les produits numériques, car **Paddle gère la TVA à ta place** et paie Madagascar. MCB reçoit les virements SWIFT (code **MCBLMGMGXXX**).

**Fait #3 (légal)** : Vendeur hors UE vendant du B2C numérique à l'UE → OSS Non-UE dès 1 €, SAUF si Merchant of Record. En **B2B avec n° de TVA client → reverse charge** (tu ne collectes pas de TVA). Pour du B2C, utiliser Paddle évite toute déclaration de TVA.

**Idée retenue (Phase 4)** : **Pack "Site vitrine / Landing page clé en main pour TPE-PME françaises"** (artisans, commerçants, coaches, professions libérales), livré en 5 jours, paiement **Payoneer (B2B, reverse charge)**, avec option maintenance mensuelle récurrente. Produit différenciateur + scalable + 0 € + encaissable MG + légalement simple. Plan B = produit numérique via Paddle.

**Réalisme** : 1er euro possible en 1-2 semaines (prospection manuelle B2B). Revenu "quotidien stable" = quelques semaines (empilement de contrats de maintenance + produit numérique). Pas de promesse de revenu passif garanti.

---

## 3 actions à faire AUJOURD'HUI
1. **Ouvrir un compte Payoneer** (avec ta pièce d'identité) et récupérer tes coordonnées de compte de réception EUR/USD → c'est le socle de l'encaissement. https://www.payoneer.com
2. **Lister 30 cibles françaises** (artisans/restaurateurs/coaches sans site ou avec site obsolète) via Google Maps France + groupes Facebook/LinkedIn francophones — à partir de la liste dans `02-idees-et-scoring.md` / `03-top3-detaille.md`.
3. **Lire `04-decision-et-plan-30j.md`** et préparer ta 1re "Payment Request" Payoneer (test avec un proche français pour valider la chaîne Payoneer → MCB avant de prospecter).

---

## Questions ouvertes / besoins de l'humain
- Confirmer auprès de MCB si ton compte accepte un compte USD/EUR (réduit les frais).
- Valider ton statut de facturation en Madagascar avec un comptable.
- Me dire si tu préfères démarrer en **B2B service** (retenu) ou **produit numérique B2C** (Plan B).
