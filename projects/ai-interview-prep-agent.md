# AI Interview Prep Agent

**Tagline :** Préparez-vous à n'importe quel entretien en 60 secondes.

---

## 🎯 Problème

Préparation d'entretien = **5-10 heures de travail**.

Résultats :
- Sources fragmentées (Glassdoor, blogs, articles divers)
- Pas de **customisation** (profil vs rôle)
- **Stresse** : manque de confiance avant l'entretien

---

## 💡 Solution

**Générateur qui produit en 60 secondes :**

Input (Company + Role) → **Claude LLM** → Output (15-page prep dossier)

Génère :
- **Company research** (culture, recent news, challenges)
- **Role requirements** (hard skills, soft skills, questions)
- **30 interview questions** (comportementales + techniques)
- **Talking points** (stories à utiliser)
- **Potential pitfalls** (ce à éviter)

---

## 🏗️ Architecture

**Stack :**
- **LLM :** Claude 3.5 Sonnet (balance vitesse/quality)
- **Backend :** FastAPI + Python
- **Frontend :** Next.js (optional, web UI)
- **Validation :** Pydantic (structure output)
- **Export :** Markdown → PDF

**Workflow :**
```
Input (Company + Role + CV optionnel)
    ↓
LLM: Generate (research + questions + strategies)
    ↓
Format + Polish
    ↓
Output: PDF téléchargeable (15 pages)
```

---

## 📊 Résultats (août 2026)

- **200+ dossiers** générés
- **60 secondes** generation time
- **90% satisfaction** utilisateur
- **70% utilisateurs** font réellement l'entretien
- **Feedback post-entretien :** "Ça m'a rendu plus confiant"

**Hypothèses validées :**
- ✅ Les gens utilisent vraiment les dossiers générés
- ✅ 60 secondes est acceptable (rapide, pas cheap)
- ✅ Les contenus générés sont utiles (pas hallucination majeure)

---

## 🎓 Leçons apprises

### ✅ Points forts

1. **Timing :** 60 secondes = sweet spot
2. **Exhaustivité :** 30Q + 15Q = suffisant
3. **Contextualisation :** Company name + role = super pertinent
4. **Format :** PDF téléchargeable > Notion/HTML (adoption)

### ❌ Défis rencontrés

1. **Hallucinations :** Première version inventait infos sur la compagnie
   - **Fix :** Prompt clairement "Research findings" vs "Questions suggérées"

2. **Qualité LLM :** Différence notable entre modèles
   - **Fix :** Utilisé Claude 3.5 (plus stable que GPT-4o)

3. **User feedback :** Au début, pas assez de detail
   - **Fix :** Ajouter explications pour chaque question

---

## 🚀 Roadmap

**Court terme :**
- [ ] Intégration LinkedIn (fetch profile data)
- [ ] Mock interview mode (questions in real-time, scoring)
- [ ] Feedback post-entretien ("Comment j'ai fait?")

**Moyen terme :**
- [ ] Community : partagez preps, apprenez des autres
- [ ] Premium : Mock interviews avec humains, 1-on-1 coaching

**Long terme :**
- [ ] 10,000+ utilisateurs/mois
- [ ] Partenariats universités et bootcamps

---

## 📚 Compétences démontrées

✅ **Productisation IA :** Idée → produit utilisé  
✅ **Performance :** 60s c'est rapide (bonne architecture)  
✅ **User feedback :** Itération rapide, écoute utilisateur  
✅ **Scalability :** Peut gérer 10,000+ utilisateurs/jour  
✅ **Limitation acknowledgment :** Clair sur hallucination risk

---

[← Retour aux projets](index.md) | [Accueil](/)
