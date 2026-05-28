# 🔍 Claude Skill — Recherche Fiscale

> Un assistant de recherche juridique en droit fiscal français pour Claude.  
> Vérifie chaque règle sur Légifrance (Open Legi) avant de répondre.

---

## Le problème que ce skill résout

Claude sans instructions précises peut citer des articles abrogés, inventer des taux, ou confondre des versions historiques de textes. En fiscalité, une erreur coûte cher.

Ce skill donne à Claude une **méthodologie rigoureuse** : reformuler d'abord, identifier les sources, vérifier sur Légifrance, citer les articles, signaler les doutes. Il ne répond pas sans avoir cherché.

---

## Ce que ça donne concrètement

Vous posez une question :
> *"La holding animatrice peut-elle bénéficier du régime mère-fille ?"*

Claude va :
1. Reformuler pour s'assurer de comprendre la question
2. Identifier les articles applicables (art. 145 et 216 CGI)
3. Interroger Open Legi pour vérifier la version en vigueur
4. Vous répondre avec les conditions, les références exactes et les limites de l'analyse

---

## Domaines couverts

IR · IS · TVA · IFI · Droits d'enregistrement · Fiscalité internationale · Procédures LPF (prescription, pénalités, recours)

---

## Installation

### Prérequis

- Compte [Claude.ai](https://claude.ai) — abonnement **Pro ou Team** recommandé
- Connecteur **Open Legi** activé : Paramètres → Outils → Open Legi → Activer

### En 3 étapes

**1. Téléchargez** ce repo (bouton Code → Download ZIP)

**2. Remplissez** `CONFIG.md` avec les informations de votre cabinet (nom, format de réponse préféré, domaines de spécialité)

**3. Créez un Projet dans Claude.ai**
   - Ouvrez Claude.ai → Projets → Nouveau projet → nommez-le "Recherche Fiscale"
   - Dans les instructions du projet, collez le contenu de `SKILL.md` puis de `CONFIG.md`

C'est tout. Posez votre première question.

> Le fichier `INSTALL.md` contient un guide plus détaillé avec des exemples de questions de test.

---

## Contenu du repo

```
skill-recherche-fiscale/
├── README.md                         ← Vous êtes ici
├── SKILL.md                          ← Instructions pour Claude (5 phases)
├── CONFIG.md                         ← À remplir : cabinet, format, domaines
├── INSTALL.md                        ← Guide d'installation détaillé
└── references/
    ├── sources-fiscales.md           ← Articles CGI/LPF/BOFiP par domaine
    └── pieges-courants.md            ← Erreurs fréquentes à éviter
```

---

## Limites importantes

Ce skill est un outil d'assistance, pas un substitut au raisonnement juridique.

- Il ne remplace pas la lecture des textes originaux sur Légifrance
- Il ne garantit pas l'exhaustivité de la jurisprudence sur un sujet
- **La responsabilité professionnelle reste celle de l'avocat ou du conseil**

Claude est instruit de signaler ses doutes plutôt que d'inventer des réponses. Si Open Legi est indisponible, il l'indique explicitement.

---

## Licence

[MIT](./LICENSE) — Utilisation libre, y compris commerciale. Citez la source si vous partagez.
