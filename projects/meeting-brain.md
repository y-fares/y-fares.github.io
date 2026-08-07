# Meeting Brain

**Tagline :** Transformez vos réunions chaotiques en actions claires.

---

## 🎯 Problème

Les réunions produisent des **comptes-rendus longs (2-3 pages) qu'on ne lit pas**.

Résultats :
- Aucune clarté sur les **décisions prises**
- Actions "confiées" sont **oubliées**
- Décideurs perdent du temps à **rédiger après la réunion**

---

## 💡 Solution

**Produit IA qui transforme automatiquement :**

Input (Audio/Transcript) → **Claude LLM** → Output (Structured)

Génère en 2-3 minutes :
- **Synthèse** (1 page)
- **Décisions** (claires, numérotées)
- **Actions** (avec owners)
- **Responsabilités** (pas d'ambiguïté)

---

## 🏗️ Architecture

**Stack :**
- **Input :** Upload audio (future) ou transcription manuelle
- **Processing :** Claude Opus pour extraction structure
- **Output :** JSON → HTML → export formats (PDF, Notion API, Slack webhook)
- **Storage :** Airtable (historique)

**Temps de traitement :** 2-3 minutes end-to-end

---

## 📊 Résultats (août 2026)

- **50+ réunions** traitées
- **85% satisfaction** utilisateur
- **20 minutes** économisées par réunion (pas besoin de rédiger)
- **2-3 min** de traitement
- **90%+ exactitude** (extraction structure)

**Hypothèses validées :**
- ✅ Les gens utilisent avec vrais sujets de réunion
- ✅ L'extraction IA est suffisamment bonne
- ✅ Formats de sortie (Notion) sont utilisés

---

## 🎓 Leçons apprises

**MVP time :** 4 semaines (parallèle avec Trending Content Engine)

**Clé du succès :** Prompt engineering bien pensé
- Tester 20+ prompt variations
- Version finale = 500 tokens, très structurée
- Extraction fiable à 90%+

**Limitation connue :** Pas de vrai audio processing (Whisper API complexe). Solution : transcription manuelle pour MVP.

---

## 🚀 Roadmap

- [ ] Intégration Zoom / Google Meet (auto-record)
- [ ] Slack commands (`/meeting-summary #channel`)
- [ ] Analytics : tracking décisions → implémentation
- [ ] 1000+ réunions traitées (fin 2026)

---

## 📚 Compétences démontrées

✅ **MVP rapide :** 4 semaines, livrable tout seul  
✅ **LLM bien utilisé :** Prompt engineering, structure output  
✅ **UX simple :** Interface minimale, focus output  
✅ **Productibilité :** Réutilisable, extensible, scalable

---

[← Retour aux projets](index.md) | [Accueil](/)
