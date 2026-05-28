# INSTALL.md — Guide d'installation en 5 minutes
# Skill : Recherche Fiscale
# Aucune compétence technique requise.

---

## Ce que fait ce skill

Ce skill transforme Claude en assistant de recherche juridique fiscale rigoureux.
Il interroge systématiquement Open Legi (Légifrance) pour vérifier chaque règle,
cite ses sources, et signale ses doutes — comme un excellent stagiaire juriste.

---

## Étape 1 — Prérequis

Vous avez besoin de :
- Un compte **Claude.ai** (Pro ou Team recommandé)
- Le connecteur **Open Legi** activé dans vos outils Claude
  → Paramètres → Outils → Rechercher "Open Legi" → Activer

---

## Étape 2 — Installer le skill

### Option A — Via un Projet Claude (recommandé)

1. Ouvrez **Claude.ai**
2. Cliquez sur **"Projets"** dans le menu gauche
3. Créez un nouveau projet : **"Recherche Fiscale"**
4. Dans les **instructions du projet**, copiez-collez intégralement le contenu
   du fichier `SKILL.md`
5. Toujours dans les instructions, ajoutez à la suite le contenu de `CONFIG.md`
   **après l'avoir rempli** avec vos informations cabinet

### Option B — Via les instructions personnalisées globales

1. Ouvrez **Claude.ai** → **Paramètres** → **Profil**
2. Dans "Préférences utilisateur", copiez le contenu de `SKILL.md` + `CONFIG.md`
3. Ce skill sera actif dans **toutes** vos conversations

> 💡 **Recommandation** : préférez l'Option A (Projet).
> Cela isole le skill dans un espace dédié et ne perturbe pas vos autres usages.

---

## Étape 3 — Configurer votre cabinet

Ouvrez le fichier `CONFIG.md` et remplissez :
- [ ] Le nom de votre cabinet
- [ ] Votre nom et titre
- [ ] Votre format de sortie préféré
- [ ] Vos domaines de spécialité
- [ ] Votre mention de fin de réponse (optionnel)

Copiez ensuite ce fichier complété à la suite du `SKILL.md` dans les instructions
de votre Projet.

---

## Étape 4 — Tester le skill

Ouvrez votre Projet et testez avec une de ces questions :

> *"Quelles sont les conditions d'application du régime mère-fille ?"*

> *"Quel est le taux de la retenue à la source sur les dividendes versés à un
> résident américain sous la convention franco-américaine ?"*

> *"Mon client n'a pas déclaré un compte bancaire en Suisse depuis 2018,
> quels sont les risques ?"*

Claude doit :
1. Reformuler la question avant de répondre
2. Interroger Open Legi (vous verrez l'indicateur de recherche)
3. Citer les articles du CGI ou LPF
4. Signaler les limites de son analyse

---

## Étape 5 — Partager avec votre équipe

Pour partager ce skill avec vos collaborateurs :
1. Envoyez-leur le dossier complet (`SKILL.md` + `CONFIG.md` rempli + `INSTALL.md`)
2. Chaque collaborateur suit les mêmes étapes 1 à 4
3. Ils peuvent personnaliser leur propre `CONFIG.md`

---

## En cas de problème

| Problème | Solution |
|---|---|
| Claude ne cite pas de sources | Vérifiez que le connecteur Open Legi est bien activé |
| Réponses trop courtes | Dans CONFIG.md, mettre `longueur : détaillée` |
| Claude ne reformule pas les questions | Relisez que le SKILL.md est bien copié intégralement |
| Open Legi indisponible | Claude doit le signaler — relancez la recherche plus tard |

---

## Questions fréquentes

**Ce skill peut-il remplacer une recherche sur Légifrance ?**
Non. Il accélère et structure la recherche, mais ne remplace pas la lecture des
textes originaux pour les dossiers à fort enjeu.

**Mes données sont-elles sécurisées ?**
Ne transmettez jamais d'informations personnelles de clients dans Claude.
Utilisez des anonymisations (Client A, Société X) pour les cas pratiques.

**Le skill fonctionne-t-il sans Open Legi ?**
Partiellement. Claude utilisera ses connaissances générales mais le signalera.
Pour une recherche fiable, Open Legi est indispensable.

---

*Skill créé pour les avocats fiscalistes et conseils fiscaux.*
*Version 1.0*
