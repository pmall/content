---
title: Intervention IA — pistes pour les questions des étudiants
format: talk-prep
status: draft
ideas: [compute-is-the-missing-picture, agent-gets-an-environment, ai-is-blurry-super-agency, explaining-tokens-from-the-corpus, less-between-data-and-result, human-work-is-compressed, orchestrating-agents-strategies, human-cost-of-ai-focus-and-senses, easy-environment-replaced-first, human-ai-already-indistinguishable]
created: 2026-10-23
sources:
  - https://www.cnn.com/2026/10/08/science/ai-biology-anthropic-dna-discovery
  - https://hebdo39.net/rubrique-grands-mots-grands-remedes-une-sortie-de-route-au-grand-prix/
  - https://www.aol.com/articles/prix-pascal-nouveau-prix-litt%C3%A9raire-095519000.html
  - https://opencode.ai/docs/go/
---

# Intervention IA : pistes

Public : étudiants à l'université (licence ou master). Exemple vécu : le projet de curation.

## 1. Toi
*Parcours*
- Inserm, puis une dizaine d'années de bioinfo, et 25 ans de code : tu as vu toutes les vagues technologiques.
- « De plus en plus expert en IA, sans savoir ce que ça veut dire. »

## 2. Comprendre l'IA
*Ce qui est important à comprendre · Distinguer l'humain de l'IA · La super IA*
- Un modèle ne « sait » rien : c'est une fonction qui prédit le prochain mot.
- Une réponse n'est qu'un tirage parmi une infinité de réponses possibles.
- Super IA ? Ça dépend de ce qu'on appelle la super IA. On ne sait déjà pas définir l'intelligence. Tu préfères parler de « super agentivité ».
- Distinguer l'humain de l'IA : on n'y arrive déjà plus. Le Prix du roman Fnac 2026 a récompensé un roman (*C'était ça ou mourir*) qu'un détecteur a jugé presque entièrement écrit par une IA. L'éditeur canadien de l'auteur a confirmé l'usage de l'IA ; l'auteur, lui, nie toujours.

## 3. S'en servir pour la science
*Prompts · Quelles IA · Abonnements · Formation*
- Un prompt oriente la prédiction. Fournir les données plutôt que solliciter la mémoire du modèle.
- Le modèle a le droit de répondre « je ne sais pas ».
- Abonnements : oui, au moins un Pro à 20 €, ou OpenCode Go (10 $/mois, 5 $ le premier mois).
- Pratiquer sur un vrai projet avant de chercher un certificat.

## 4. L'IA dans un labo
*Reproductibilité · Freins · Hypothèses*
- Le projet de curation, presque terminé : de 200 M à 57 M de tokens envoyés au modèle pour 100 publications après optimisation (exemple d'astuce : sous zsh, `echo ===` plante, et l'agent perd un tour à chaque fois). L'agent décide, le code vérifie, « non tranché » vaut mieux que faux, et la surveillance reste possible.
- Les freins sont surtout humains et organisationnels.
- Un agent par hypothèse : l'exhaustivité devient une question d'énergie.

## 5. Science et biotech
*Révolution scientifique · Impact sur les biotechs*
- C'est une question de calcul : produire, évaluer, corriger en boucle.
- La valeur se déplace vers des données bien présentées pour un agent.
- Accroche d'actualité : les agents d'Anthropic auraient trouvé un système de type CRISPR chez des phages. Découverte contestée.

## 6. L'avenir
*Ce que l'IA va remplacer · Peur*
- Plus un environnement est facile à mettre en place, plus le travail sera remplacé. Un avocat ou un médecin : leur environnement, c'est essentiellement l'accès à une base de connaissances.
- Certain de la destination, beaucoup de frictions sur le chemin.
- Peur ? Non, pas du tout. Ce que tu prédis, en revanche : le « burn-out de focus » et la surcharge sensorielle.
