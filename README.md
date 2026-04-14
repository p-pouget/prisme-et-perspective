# Prisme et perspective

## Lab de Restitution - Architecture & Flux

Interface d’exposition technique pour l’archivage de flux de données et la documentation d’architectures logicielles. Cette plateforme centralise les preuves techniques d'extractions, de manipulations de flux et de déploiements.

## MÉTHODOLOGIE

Le rendu est piloté par la donnée (Data-Driven Rendering). Le contenu n'est pas rédigé manuellement mais généré par la transformation de flux JSON en rapports statiques via le framework Astro.

1. **Source** : Ingestion de fichiers JSON structurés dans le répertoire de données.
2. **Mapping** : Utilisation de `getStaticPaths` pour itérer sur les objets et créer les routes dynamiques.
3. **Restitution** : Génération de pages statiques (SSG)

## ARBORESCENCE

- **/src/data/** : Dépôt des flux JSON. Source de vérité unique contenant les données extraites.
- **/src/pages/** : Templates de génération dynamique des rapports de restitution (ex: `[id].astro`).
- **/src/layouts/** : Structures d'exposition. Définit les environnements visuels pour les analyses de flux.
