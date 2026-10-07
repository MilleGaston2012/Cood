# Cood

Cood est un organiseur natif pour macOS qui rassemble tâches, devoirs, notes et raccourcis vers les fichiers. L’espace de travail reste enregistré sur le Mac, sans compte ni abonnement.

## Fonctionnalités

- **Aujourd’hui** : aperçu des éléments à traiter.
- **Boîte de réception** : capture rapide avec **⌘N**.
- **Tâches** : création et suivi des tâches.
- **Devoirs** : matière, date d’échéance, consignes et état terminé.
- **Notes** : éditeur enrichi avec police, taille, alignement, tableaux, séparateurs et sauvegarde automatique. Nouvelle note avec **⌘⇧N**.
- **Fichiers** : raccourcis ouverts avec les apps macOS habituelles.
- **Recherche locale** et suggestions fondées sur des règles simples.
- **Mises à jour** : vérification quotidienne discrète de la dernière release GitHub.

## Télécharger et installer

La version **0.1.2** ajoute les réglages accessibles depuis le menu macOS et la page d’accueil, ainsi que des zones cliquables agrandies. Elle cible les Mac Apple Silicon (M1 ou ultérieur), en arm64, sous macOS 14 Sonoma ou ultérieur. Téléchargez `Cood-0.1.2-macOS-Apple-Silicon-arm64.dmg`, ouvrez-le, puis faites glisser Cood dans le dossier **Applications**. Les Mac Intel ne sont pas pris en charge.

Cette application n’est pas notariée par Apple ; macOS peut afficher un avertissement au premier lancement.

## Données et confidentialité

Les données de l’espace de travail sont enregistrées localement dans `~/Library/Application Support/Cood/workspace.json`. Les fichiers ajoutés restent à leur emplacement d’origine : Cood conserve des raccourcis vers eux.

Au lancement, le vérificateur contacte l’API publique de GitHub au plus une fois par jour pour chercher une release plus récente. Il n’envoie pas le contenu de l’espace de travail. Si un DMG Apple Silicon est joint à la release, Cood propose de le télécharger ; il faut ensuite remplacer l’app dans Applications.

Les suggestions sont calculées localement ; Cood n’embarque pas de modèle d’intelligence artificielle.

## Compiler depuis les sources

L’archive `Cood-source.zip` est attachée à la [dernière release](https://github.com/MilleGaston2012/Cood/releases/latest). Sur un Mac équipé de Swift et des outils de développement Apple, décompressez-la et lancez `./scripts/make-app.sh`. Le script construit l’application pour arm64 et macOS 14 ou ultérieur.

## Limites actuelles

Cood ne se synchronise pas avec Calendrier, Rappels, Mail ou Notes d’Apple. Les suggestions restent locales et fondées sur des règles simples.
