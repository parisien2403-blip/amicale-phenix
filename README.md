# Trésorerie — Amicale du Phénix du 4ᵉ RIISC

Application locale pour la tenue de la trésorerie de l'association : recettes, dépenses, comptage de caisse, suivi de banque et liste des cotisants.

## Utilisation

1. Téléchargez le fichier `index.html` (ou clonez ce dépôt).
2. Double-cliquez sur `index.html` pour l'ouvrir dans votre navigateur (Chrome, Firefox, Edge...). Aucune installation n'est nécessaire.
3. Toutes les données sont enregistrées **uniquement dans ce navigateur, sur cet ordinateur** (technologie *localStorage*). Rien n'est envoyé sur internet.

⚠️ **Important** : si vous videz le cache du navigateur, changez d'ordinateur ou de navigateur, les données ne seront pas présentes. Pensez à utiliser régulièrement le bouton **« Télécharger une sauvegarde (.json) »** dans l'onglet *Données*, et à conserver ce fichier en lieu sûr (clé USB, e-mail à vous-même, etc.). Vous pourrez le restaurer à tout moment avec **« Restaurer une sauvegarde »**.

## Fonctionnalités

- **Tableau de bord** : nombre de cotisants, cotisants à jour, total des cotisations, total recettes, total dépenses, résultat cumulé, total stock, soldes théoriques de caisse/banque, et un **total général** (recettes + cotisations + stock − dépenses) mis en avant en haut de l'application.
- **Recettes** : enregistrement des recettes liées aux prestations (libellé libre), avec date, montant et moyen de paiement. Recherche, filtre par période, export Excel.
- **Dépenses** : même principe, avec un libellé destiné par exemple au nom du magasin ou du fournisseur.
- **Caisse** : comptage du nombre de billets, de pièces et de chèques détenus, calcul automatique du total, historique des comptages avec écart par rapport au solde théorique (calculé à partir des recettes/dépenses en espèces).
- **Banque** : solde théorique calculé à partir des opérations par chèque/virement/carte, et historique des relevés bancaires réels avec écart.
- **Stock** : suivi des denrées (boissons, chips...) avec quantité et prix unitaire ; le montant total par denrée et la valeur totale du stock sont calculés automatiquement. Export Excel.
- **Cotisants** : import d'un fichier Excel (colonnes Nom, Prénom et Montant), ajout/modification manuelle, statut « à jour » déduit automatiquement dès qu'un montant est renseigné, export Excel.
- **Bilan** : génère un bilan de trésorerie sur une période choisie (solde en début/fin de période pour la caisse et la banque, détail des opérations, situation actuelle), à imprimer ou enregistrer en PDF — pratique pour le présenter à la banque.
- **Données** : export/import d'une sauvegarde complète (.json), réinitialisation.

## Exporter le bilan en PDF

Dans l'onglet **Bilan**, choisissez une période puis cliquez sur **« Imprimer / Enregistrer en PDF »**. Dans la fenêtre d'impression qui s'ouvre, sélectionnez comme imprimante **« Enregistrer au format PDF »** (Chrome/Edge) ou **« Microsoft Print to PDF »** (Windows) plutôt qu'une imprimante physique, puis validez. Aucune connexion internet n'est nécessaire pour cette étape.

## Format du fichier Excel pour l'import des cotisants

Idéalement, la première ligne doit contenir des en-têtes parmi :

| Nom | Prénom | Montant |
|---|---|---|

Seules les colonnes **Nom** et **Prénom** sont indispensables. Si le fichier n'a pas d'en-tête reconnu, l'application suppose l'ordre **Nom, Prénom, Montant**.

## Hébergement sur GitHub Pages (facultatif)

Si vous activez GitHub Pages sur ce dépôt (Settings → Pages → Source: branche `main`), vous pourrez ouvrir l'application depuis une adresse web, sans avoir à télécharger le fichier. Attention : les données restent malgré tout stockées localement dans le navigateur utilisé, et ne sont pas partagées entre plusieurs ordinateurs.

## Structure du dépôt

- `index.html` — l'application complète (HTML, CSS et JavaScript dans un seul fichier).
- `README.md` — ce document.
- `logo_phenix.ico`, `logo_phenix_512.png`, `logo_phenix_256.png` — icône du Phénix, à utiliser pour personnaliser le raccourci de l'application sur le bureau.

## Licence

Libre d'utilisation et de modification pour les besoins de l'association.
