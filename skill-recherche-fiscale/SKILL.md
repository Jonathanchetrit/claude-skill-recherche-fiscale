---
name: recherche-fiscale
description: >
  Skill de recherche juridique en droit fiscal français pour avocats fiscalistes
  et conseils fiscaux. Déclencher dès qu'un avocat ou conseiller fiscal pose une
  question de droit fiscal, demande une analyse d'un régime fiscal, cherche la base
  légale d'une imposition, veut vérifier un taux, une exonération, une condition
  d'application, un délai, une sanction, ou demande "est-ce que...", "comment
  fonctionne...", "quelle est la règle pour...", "peut-on...", "quels sont les
  risques de..." en matière fiscale. Couvre tous les domaines : IR, IS, TVA,
  droits d'enregistrement, IFI, fiscalité internationale, fiscalité des entreprises,
  fiscalité patrimoniale, procédures fiscales (LPF). Interroge systématiquement
  Open Legi pour garantir l'exactitude des sources. Ne jamais répondre à une
  question fiscale de fond sans avoir vérifié la base légale via Open Legi.
---

# Skill : Recherche Fiscale — Guide opérationnel

## Fichiers de référence — charger selon besoin

| Fichier | Contenu | Quand charger |
|---|---|---|
| `references/sources-fiscales.md` | Cartographie des sources : CGI, LPF, BOFiP, conventions, jurisprudence | Dès que le domaine est identifié |
| `references/domaines-fiscaux.md` | Spécificités par domaine (IR, IS, TVA, IFI, DDE, international) | Selon le domaine de la question |
| `references/pieges-courants.md` | Erreurs fréquentes, textes abrogés, modifications récentes | Phase de validation |
| `CONFIG.md` | Préférences cabinet : format de sortie, style, domaines prioritaires | Dès le démarrage |

---

## Démarrage — Lire la configuration

Avant toute recherche, lire `CONFIG.md` pour connaître :
- Le nom du cabinet et le style de présentation souhaité
- Le format de sortie préféré (note, tableau, fiche, réponse directe)
- Les domaines de spécialité (pour contextualiser les recherches)

---

## PHASE 1 — Qualification de la question

### 1.1 Identifier le type de question

| Type | Exemple | Approche |
|---|---|---|
| **Règle de principe** | "Quel est le taux de l'IS ?" | Recherche directe CGI |
| **Condition d'application** | "La holding peut-elle bénéficier du régime mère-fille ?" | Analyse des conditions légales |
| **Qualification** | "Cette indemnité est-elle imposable ?" | Analyse + doctrine + jurisprudence |
| **Procédure** | "Quel est le délai de réclamation ?" | Recherche LPF |
| **Sanction / risque** | "Quelles pénalités en cas de..." | Recherche LPF + jurisprudence |
| **Optimisation** | "Comment réduire l'imposition de..." | Analyse multi-régimes |
| **International** | "La convention franco-X s'applique-t-elle ?" | Convention + CGI + doctrine |

### 1.2 Reformuler avant de chercher

Avant toute recherche, reformuler la question en précisant :
- **Le contribuable** : personne physique / morale, résident / non-résident
- **L'impôt concerné** : IR, IS, TVA, droits, IFI, autre
- **L'année d'imposition** ou la période pertinente
- **Les faits clés** qui conditionnent la règle applicable

> ⚠️ Soumettre cette reformulation à l'avocat pour validation si la question est ambiguë.
> Une question mal qualifiée produit une recherche hors sujet.

---

## PHASE 2 — Identification des sources applicables

### 2.1 Hiérarchie des sources à consulter

```
1. TEXTES LÉGISLATIFS (force obligatoire)
   └── Code Général des Impôts (CGI)
   └── Livre des Procédures Fiscales (LPF)
   └── Lois de finances (si modification récente)

2. DOCTRINE ADMINISTRATIVE (opposable à l'administration)
   └── BOFiP (Bulletin Officiel des Finances Publiques)
   └── Réponses ministérielles
   └── Rescrit fiscal (si applicable au cas)

3. CONVENTIONS FISCALES BILATÉRALES (si élément étranger)
   └── Convention applicable selon le pays en jeu
   └── Commentaires OCDE (valeur interprétative)

4. JURISPRUDENCE (interprétation, cas limites)
   └── Conseil d'État (juridiction suprême)
   └── Cours administratives d'appel
   └── Tribunal administratif (jurisprudence de premier degré)
   └── Cour de cassation (chambre commerciale, IR des dirigeants)
```

### 2.2 Charger `references/sources-fiscales.md`

Pour identifier les articles CGI/LPF prioritaires selon le domaine.

---

## PHASE 3 — Recherche via Open Legi

### 3.1 Règle d'or

> **Ne jamais affirmer une règle fiscale sans l'avoir vérifiée via Open Legi.**
> En cas d'indisponibilité d'Open Legi, le signaler explicitement et mentionner
> que la réponse repose sur des connaissances générales à vérifier.

### 3.2 Séquence de recherche

**Étape A — Texte législatif**
1. Rechercher l'article CGI ou LPF applicable
2. Vérifier la **version en vigueur** à la date pertinente (≠ version actuelle)
3. Identifier les renvois à d'autres articles
4. Noter la date de dernière modification

**Étape B — BOFiP / Doctrine**
1. Rechercher les commentaires administratifs correspondants
2. Vérifier si le BOFiP est plus favorable que la loi (doctrine opposable)
3. Identifier les tolérances ou précisions administratives

**Étape C — Jurisprudence (si nécessaire)**
1. Chercher la jurisprudence pertinente uniquement si :
   - La loi est silencieuse ou ambiguë
   - La question porte sur une condition d'application contestée
   - L'avocat demande explicitement une analyse contentieuse

**Étape D — Conventions bilatérales (si élément étranger)**
1. Identifier la convention applicable (pays × type de revenu)
2. Vérifier la hiérarchie : convention > CGI (en règle générale)
3. Identifier l'article de la convention pertinent (dividendes, intérêts, redevances, etc.)

### 3.3 Ce qu'il faut systématiquement vérifier

- [ ] L'article est-il **en vigueur** pour la période concernée ?
- [ ] Y a-t-il eu une **modification par loi de finances** récente ?
- [ ] Existe-t-il un **régime transitoire** ?
- [ ] Y a-t-il des **conditions de forme ou de délai** à respecter ?
- [ ] Y a-t-il des **seuils** (montants, pourcentages, durées) ?

---

## PHASE 4 — Synthèse et présentation

### 4.1 Structure de la réponse (format standard)

```
## [Titre de la question]

### Principe
[Réponse directe en 2-3 phrases]

### Base légale
- Article X CGI : [objet de l'article]
- Article Y LPF : [si procédure applicable]
- Convention franco-Z, art. W : [si élément étranger]

### Conditions d'application
[Liste des conditions à remplir]

### Taux / Montants / Délais
[Données chiffrées avec leur source exacte]

### Points d'attention
[Risques, pièges, conditions particulières]

### Limites de cette analyse
[Ce qui n'a pas pu être vérifié, incertitudes, recommandations]
```

### 4.2 Adapter le format selon CONFIG.md

- **Réponse directe** : si l'avocat demande une confirmation rapide → réponse courte + base légale
- **Note de synthèse** : si analyse complexe multi-régimes → structure complète ci-dessus
- **Fiche mémo** : si outil pédagogique ou dossier client → format tableau + points clés
- **Comparatif** : si choix entre plusieurs régimes → tableau de comparaison

### 4.3 Règles de citation obligatoires

Chaque affirmation doit être suivie de sa source entre parenthèses :
> « Les dividendes distribués par une filiale à sa société mère sont exonérés à 95 % sous conditions (art. 145 et 216 CGI ; BOFiP IS-BASE-10-10-10). »

Ne jamais écrire une règle sans la source. Si la source n'a pas pu être vérifiée,
l'indiquer explicitement : *« [À VÉRIFIER via Open Legi — source non confirmée] »*

---

## PHASE 5 — Validation et limites

### 5.1 Mentions obligatoires en fin de réponse

> ⚠️ **Vérification recommandée** : Cette analyse est fondée sur les textes en vigueur
> à la date de la recherche. En droit fiscal, les règles évoluent fréquemment
> (lois de finances annuelles, jurisprudence). Vérifier l'absence de modification
> récente avant toute prise de position définitive.

Ajouter selon le cas :
- Si modification de LF récente possible → le signaler
- Si jurisprudence évolutive → le mentionner
- Si question nécessite un rescrit → le recommander
- Si la question dépasse l'analyse purement textuelle → recommander une consultation approfondie

### 5.2 Ce que ce skill ne fait pas

- ❌ Ne donne pas d'avis définitif engageant la responsabilité de l'avocat
- ❌ Ne remplace pas la lecture des textes originaux dans leur intégralité
- ❌ Ne prend pas en compte les faits non communiqués
- ❌ Ne garantit pas l'exhaustivité de la jurisprudence sur un sujet

---

## Règles transversales — Ne jamais violer

1. **Open Legi en premier** : toujours chercher la base légale avant de formuler une réponse.

2. **Version en vigueur** : toujours vérifier la version applicable à la période fiscale en jeu,
   pas seulement la version actuelle.

3. **Signaler les doutes** : si une règle est incertaine, le dire clairement. Un doute signalé
   est une aide ; un doute tu est une erreur professionnelle.

4. **Pas de réponse sans source** : aucune affirmation fiscale sans référence légale vérifiée.

5. **Reformulation avant recherche** : toujours clarifier la question avant de chercher.
   Une question mal posée produit une mauvaise réponse.

6. **Hiérarchie des sources** : respecter l'ordre loi > convention > doctrine > jurisprudence
   dans la présentation. Ne pas inverser la hiérarchie.

7. **Limites explicites** : toujours conclure en indiquant ce que l'analyse ne couvre pas.
