# Cood

Cood est un organiseur natif pour macOS, conçu pour rassembler les tâches, les devoirs, les notes et les fichiers dans une interface simple et rapide. L’application stocke son espace de travail sur le Mac et fonctionne sans compte ni service en ligne.

## Fonctionnalités

- **Aujourd’hui** : aperçu des éléments à traiter.
- **Boîte de réception** : capture rapide avec **⌘N**.
- **Tâches** : création et suivi de tâches.
- **Devoirs** : matière, date d’échéance, détails et état terminé.
- **Notes** : éditeur avec choix de police et de taille, alignement, tableaux, séparateurs et sauvegarde automatique. Nouvelle note avec **⌘⇧N**.
- **Fichiers** : raccourcis vers des fichiers et dossiers, ouverts avec les fonctions de macOS.
- **Recherche locale** et suggestions fondées sur des règles simples.

## Télécharger et installer

La version prête à l’emploi est disponible dans les [releases](https://github.com/MilleGaston2012/Cood/releases). Téléchargez le fichier **Cood-0.1.0-macOS-Apple-Silicon-arm64.dmg**, ouvrez-le, puis faites glisser Cood dans le dossier **Applications**.

Au premier lancement, macOS peut afficher un avertissement car cette version n’est pas notariée par Apple. Le DMG est destiné aux Mac Apple Silicon ; il est compilé en arm64.

## Compatibilité

- Mac avec puce Apple Silicon **M1 ou ultérieure**
- **macOS 14 Sonoma ou ultérieur**
- Les Mac Intel ne sont pas pris en charge par cette version.

## Données et confidentialité

Cood n’utilise ni compte, ni serveur, ni abonnement. Les données de l’espace de travail sont enregistrées localement dans :

```
~/Library/Application Support/Cood/workspace.json
```

Les suggestions sont produites par des règles locales ; Cood n’embarque pas de modèle d’intelligence artificielle. Les fichiers ajoutés à la section Fichiers restent à leur emplacement d’origine : Cood conserve des raccourcis et les ouvre avec macOS.

## Compiler depuis les sources

Le code source est fourni dans l’archive **Cood-source.zip** attachée à la [release](https://github.com/MilleGaston2012/Cood/releases/latest). Sur un Mac équipé des outils de développement Apple et de Swift, décompressez l’archive, ouvrez un terminal dans le dossier du projet et lancez :

```sh
./scripts/make-app.sh
```

Le script construit l’application pour arm64 et macOS 14 ou ultérieur.

## Limites actuelles

Cood ne se synchronise pas avec Calendrier, Rappels, Mail ou Notes d’Apple et ne se connecte pas à des services tiers. Les suggestions restent locales et fondées sur des règles simples.

## Licence

Aucune licence open source n’est encore publiée dans ce dépôt. Contactez le mainteneur avant toute redistribution ou réutilisation du code.
