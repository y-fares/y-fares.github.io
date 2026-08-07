# Trending Content Engine

## Produit IA de veille stratégique

Trending Content Engine aide les créateurs, solopreneurs et petites marques à détecter plus tôt les tendances pertinentes et à les transformer en idées de contenus actionnables.

## Problème

La veille est dispersée entre plusieurs sources. Les utilisateurs passent du temps à collecter et trier l'information, puis identifient souvent les sujets lorsqu'ils sont déjà saturés.

## Solution

Le MVP automatise la chaîne suivante :

```text
Sources publiques et flux RSS
        ↓
Collecte automatisée avec n8n
        ↓
Centralisation dans Airtable
        ↓
Résumé, classification et scoring par IA
        ↓
Regroupement en tendances
        ↓
Génération d'idées de contenus
        ↓
Consultation et validation dans Softr
```

## Rôle

**Product Owner, chef de projet IA & automatisation, concepteur du MVP**

J'ai pris en charge :

- le cadrage du problème utilisateur ;
- la proposition de valeur et la priorisation du MVP ;
- le modèle de données Airtable ;
- la conception des workflows n8n ;
- l'intégration des traitements IA ;
- la gestion des erreurs et des reprises ;
- les arbitrages liés aux API, au budget et au délai ;
- la préparation de la démonstration et de la soutenance.

## Fonctionnalités du MVP

- collecte automatisée de signaux ;
- détection des doublons ;
- résumé automatique ;
- classification thématique ;
- extraction de mots-clés ;
- scoring de pertinence et de confiance ;
- normalisation des sujets ;
- regroupement en tendances ;
- génération d'idées de contenus ;
- validation humaine via Softr.

## Stack

**Airtable · n8n · Make · Softr · Gemini · OpenAI · Claude**

## Décisions produit

- privilégier des sources simples et fiables plutôt qu'un scraping massif ;
- séparer collecte, enrichissement et regroupement pour isoler les erreurs ;
- migrer progressivement de Make vers n8n pour réduire la dépendance aux crédits ;
- conserver un humain dans la boucle pour la validation éditoriale ;
- sortir la récupération exhaustive des données LinkedIn du MVP en raison des contraintes d'API.

## Problèmes techniques résolus

### Airtable — erreurs 422

Reconstruction et sécurisation des formules de recherche afin d'éviter les requêtes invalides et de fiabiliser la détection des doublons.

### Gemini — sorties JSON

Correction du format de réponse, ajout d'un schéma structuré, nettoyage des réponses et conversion explicite des champs avant écriture dans Airtable.

### Valeurs nulles et champs numériques

Ajout de contrôles, valeurs de repli et transformations typées afin d'empêcher les données incomplètes de bloquer les workflows.

### Limites Reddit et LinkedIn

Réduction de la fréquence des appels Reddit et arbitrage explicite du périmètre LinkedIn plutôt que maintien d'une promesse techniquement fragile.

## Compétences démontrées

- cadrage produit ;
- conception de MVP ;
- architecture NoCode ;
- orchestration de workflows ;
- intégration de LLM ;
- structuration de sorties JSON ;
- gestion des erreurs ;
- arbitrage produit et technique ;
- documentation et présentation d'une solution métier.

## Statut

MVP en construction dans le cadre du bootcamp **Chef de projet IA & NoCode — Oreegami, 2026**.

Les prochaines preuves à consolider sont les métriques d'usage, les captures d'écran, une vidéo de démonstration et un retour utilisateur documenté.
