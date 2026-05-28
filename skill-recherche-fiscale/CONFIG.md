# CONFIG.md — Configuration cabinet
# À remplir une seule fois. Ce fichier est lu automatiquement par le skill.
# Remplacez chaque valeur entre [ ] par vos informations.

---

## Identité du cabinet

```
Nom du cabinet       : [Ex. : MARTIN SOPHIE AVOCATE / CABINET DUPONT FISCALITÉ]
Nom de l'avocat      : [Ex. : Sophie MARTIN]
Titre                : [Avocat à la Cour / Avocat associé / Counsel / ...]
Barreau              : [Ex. : Barreau de Paris]
Email professionnel  : [votre@email.com]
```

---

## Format de sortie préféré

Indiquer le format par défaut pour les réponses de recherche fiscale :

```
Format par défaut    : [note_synthese / reponse_directe / fiche_memo / comparatif]
                       → note_synthese  : analyse complète avec sections
                       → reponse_directe: réponse courte + base légale (questions simples)
                       → fiche_memo     : tableau + points clés (usage client ou dossier)
                       → comparatif     : tableau de comparaison (choix entre régimes)

Longueur préférée    : [concise / standard / détaillée]
Langue               : [français]
Inclure jurisprudence: [oui / non / si_pertinente]
```

---

## Domaines de spécialité

Cocher les domaines principaux du cabinet (aide à contextualiser les recherches) :

```
Domaines prioritaires:
  [ ] Fiscalité des particuliers (IR, IFI, plus-values)
  [ ] Fiscalité des entreprises (IS, TVA, intégration fiscale)
  [ ] Fiscalité internationale (conventions, prix de transfert, expatriés)
  [ ] Fiscalité patrimoniale (transmission, donation, succession)
  [ ] Contrôle fiscal et contentieux (LPF, procédures)
  [ ] Fiscalité immobilière (SCI, LMNP, promotion)
  [ ] Restructurations et fusions-acquisitions
  [ ] Autre : [préciser]
```

---

## Mentions de fin de réponse

Texte à ajouter automatiquement en fin de chaque réponse (optionnel) :

```
Mention standard     : [Ex. : "Cette analyse est fournie à titre informatif.
                        Pour une prise de position définitive, contactez le cabinet
                        au [email]."]

Mention abrégée      : [Ex. : "Analyse à vérifier avant toute décision définitive."]

Pas de mention       : [ ] Cocher si aucune mention souhaitée
```

---

## Instructions spéciales

```
Instructions libres  : [Ex. : "Toujours mentionner si un rescrit est recommandable."
                               "Mettre en gras les taux et montants clés."
                               "Toujours indiquer si la règle a changé en LFI 2024."
                               "Format bilingue français/anglais pour les clients étrangers."]
```

---

*Ce fichier CONFIG.md est lu au démarrage de chaque session.
Modifiez-le à tout moment pour adapter le comportement du skill.*
