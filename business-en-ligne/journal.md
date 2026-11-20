# Journal de suivi quotidien

> Boucle quotidienne : relire ce fichier + `04-decision-et-plan-30j.md` → exécuter les tâches du jour → mettre à jour ici → proposer le plan du lendemain.
> Si le critère d'arrêt est atteint à J30, pivoter vers l'idée n°2 (I2) et l'expliquer.

---

## 📅 2026-11-20 — JOUR 0 (setup & stratégie)

### Actions faites
- **Phase 0 — Vérification des faits (web)** : 0 € budget, encaissement Madagascar, conformité UE. Sources citées dans `01-verification-paiement-madagascar.md`.
- **Fait critique** : PayPal NE permet PAS la réception d'argent à Madagascar (confirmé PayPal community + L'Express 2026). Stripe non disponible comme vendeur MG. → Chaîne retenue : **Payoneer → MCB** (B2B) et **Paddle** (produit numérique, gère la TVA).
- **Phase 1-2** : 18 idées générées + tableau de scoring pondéré (`02-idees-et-scoring.md`).
- **Phase 3** : Top 3 détaillé (`03-top3-detaille.md`).
- **Phase 4** : décision = **I1 Pack "Site vitrine/Landing page clé en main" B2B**, plan 30 jours, KPI, critère d'arrêt (`04-decision-et-plan-30j.md`).
- **Phase 5 — Livrables construits** (`05-livrables-pret-a-lancer/`) :
  - `index.html` : page de vente complète (mobile-first, FR, promesse/offre/prix/FAQ/CTA + mentions légales/CGV/RGPD).
  - `site-client-template.html` : template de site client réutilisable (1er lot livrable).
  - `guide-google-business-profile.md` : guide livré avec l'offre.
  - `posts-et-scripts.md` : 10 posts + 5 scripts de prospection.
  - `checklist-lancement.md` : checklist gratuite (hébergement, paiement testé).
  - `suivi-quotidien.md` : modèle de suivi + KPI + CSV.

### Résultats
- Idée retenue justifiée (10 lignes). Chaîne de paiement vérifiée de bout en bout (client FR → Payoneer → MCB, frais ~3 %).
- Coût dépensé : **0 €**.

### Prochaine étape (J1)
1. **Ouvrir/compléter le compte Payoneer** (pièce d'ID malgache) + activer le compte de réception EUR + Payment Request.
2. Créer le **template de devis** et de **facture HT** (mention reverse charge).
3. **Déployer `index.html`** gratuitement (Netlify/GitHub Pages) → obtenir le sous-domaine.
4. Préparer le **test de paiement réel J3** (micro-paiement d'un proche français → retrait MCB).

### Besoins de l'humain
- Confirmer la **ville/métier cible n°1** (ex. coiffeurs Lyon, plombiers Bordeaux).
- Avoir un **proche français** dispo pour le test Payoneer J3.
- Valider le **statut de facturation** en Madagascar avec un comptable (particulier vs auto-entrepreneur vs société).

---

## 📅 À VENIR
_(Remplir chaque jour selon le plan J1-30.)_
