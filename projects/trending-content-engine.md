# Trending Content Engine

**Tagline :** Détectez les tendances avant vos concurrents. Publiez au bon moment avec les bons angles.

---

## 🎯 Problème traité

Les créateurs de contenu passent **10+ heures/semaine en veille fragmentée**.

Résultats :
- Identifient les tendances **trop tard** (après les premiers movers)
- Sources fragmentées (5+ outils différents)
- **Impossible de prioriser** les signaux (trop d'infos)
- Pas d'**angles différenciants**

---

## 💡 Solution

**Produit IA qui :**

1. **Collecte** automatiquement 500+ signaux/jour (5 sources)
2. **Enrichit** par LLM (résumé, catégorisation, mots-clés, sentiment)
3. **Regroupe** les signaux proches en tendances
4. **Transforme** en idées de contenu actionnables
5. **Expose** dans interface simple (Softr)

---

## 🏗️ Architecture

```
Collect (RSS, Google News, Reddit)
    ↓
Deduplicate (SQL)
    ↓
Enrich (Claude 3.5 Sonnet LLM)
    ↓
Store (Airtable)
    ↓
Cluster (Python grouping)
    ↓
Score (Pertinence + confiance)
    ↓
Render (Softr UI)
```

**Technologies :**
- **Orchestration :** n8n (flows, triggers, transformations)
- **Storage :** Airtable (base de données + workflows)
- **LLM :** Claude 3.5 Sonnet (enrichissement)
- **Interface :** Softr (no-code dashboard)
- **Backup :** GitHub + CSV exports

---

## 📊 Résultats (août 2026)

- **500+ signaux** collectés par jour
- **15-20 tendances** détectées par jour
- **30+ utilisateurs** testeurs actifs
- **80% sentiment positif** dans feedback
- **MVP time :** 6 semaines

**Hypothèses validées :**
- ✅ Créateurs VEULENT une solution d'agrégation de veille
- ✅ L'IA peut regrouper les signaux et créer du contexte
- ⚠️ Reach real-time (Reddit/LinkedIn) compliqué (rate limits)

---

## 🎓 Leçons apprises

### ✅ Ce qui a marché

1. **MVP-first :** Commencer avec 5 sources simples (RSS) avant Reddit/LinkedIn complexe
2. **LLM bien prompté :** Un bon prompt = 50% du travail
3. **Airtable comme centrale :** Plus simple qu'une vraie API
4. **User feedback tôt :** Testeurs ont proposé des idées inattendues

### ❌ Ce qui n'a pas marché

1. **LinkedIn API :** Trop limitée (rate limits), pas viable
2. **Clustering naïf :** Première approche (word embedding) trop lente
3. **Over-engineering interface :** Softr suffisait, pas besoin React custom

---

## 🚀 Roadmap

**Q4 2026 :**
- [ ] Deploy interface Softr complète
- [ ] Ajouter YouTube trending
- [ ] User testing approfondi (10 utilisateurs, 4 semaines)

**2027 :**
- [ ] Pricing model défini
- [ ] Intégration Slack/Discord
- [ ] 100 utilisateurs actifs

---

## 📚 Compétences démontrées

✅ **Product Management :** Découvery complète → design → build → iterate  
✅ **IA générative :** LLM responsable, prompt engineering, gestion limites  
✅ **Automatisation :** Pipelines n8n, orchestration robuste, gestion erreurs  
✅ **Architecture :** Scalabilité pensée dès le départ  
✅ **Communication :** Documentation clear, arbitrage transparent

---

[← Retour aux projets](index.md) | [Accueil](/)
