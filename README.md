# Fonctions

## one_hot_encoder
Transforme les variables catégorielles en variables numériques via one-hot encoding.
Retourne le DataFrame encodé et la liste des nouvelles colonnes créées.

## application_train_test
Charge, nettoie et fusionne les données train/test puis crée des variables financières (ratios).
Produit un dataset client enrichi prêt pour la modélisation.

## bureau_and_balance
Combine l’historique des crédits externes et leurs statuts mensuels, puis agrège au niveau client.
Génère des indicateurs globaux + spécifiques (crédits actifs et clôturés).

## previous_applications
Analyse les anciennes demandes de crédit et crée des statistiques client (montants, acceptation, refus).
Ajoute des features différenciées entre demandes approuvées et refusées.

## pos_cash
Agrège les historiques mensuels des crédits POS/Cash pour mesurer retards et activité.
Produit des indicateurs de comportement de paiement court terme.

## installments_payments
Construit des variables comportementales (retards, respect des paiements, écarts).
Crée des features très prédictives du défaut basées sur le remboursement réel.

## credit_card_balance
Agrège les transactions de cartes de crédit pour capturer l’utilisation et la variabilité financière.
Produit un profil global du comportement carte au niveau client.