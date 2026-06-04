# Séance 21 - Moments importants

## Intention de la séance

Je montre comment je m'organise après la signature d'un client. Le sujet n'est pas seulement de créer une solution IA, mais de piloter le projet : garder le client informé, cadrer le périmètre, envoyer des présentations propres, récupérer les retours, transformer les retours en tâches Codex, tester, livrer et préparer la suite sans forcer.

## Fil conducteur

1. Le silence crée le doute.
2. Le projet doit être visible.
3. Je valorise mon travail au lieu d'envoyer seulement un lien.
4. Je cadre le client, parce qu'il demandera souvent des ajouts.
5. Je livre une V1 rapidement pour récupérer les retours.
6. Je transforme chaque retour en checklist.
7. Je fais tester la solution au client.
8. Je garde une mémoire propre : présentations, calls, projet.

## Timeline de la séance

| Moment | Sujet | À transformer dans le support |
|---|---|---|
| 00:00 | Introduction : organisation, tips et satisfaction client | Hero + promesse de séance |
| 00:25 | Le silence crée le doute | Règle de communication |
| 01:02 | Le projet doit être visible | Présentation comme fil rouge |
| 01:29 | Valoriser son travail | Section sur posture et confiance |
| 01:55 | Audit, cadrage, V1, retours, V2, tests, livraison | Timeline principale |
| 03:22 | Relance tous les 3 jours | Rythme client |
| 04:14 | Exemple de relance après V1 | Messages à copier |
| 05:31 | Mettre la personne au-dessus en copie si besoin | Protection projet |
| 06:30 | Répondre en moins de 24 h | SLA simple |
| 07:26 | Présentation projet dès le début | Cadrage GitHub |
| 08:33 | Prompt Codex de cadrage | Prompt à copier |
| 09:49 | Garder la présentation dans le dossier pour enrichir Codex | Mémoire IA |
| 10:40 | Reprendre le design de l'audit | Expérience client |
| 12:31 | Erreur : petite mission non facturée | Piège fréquent |
| 13:03 | Message pour facturer un ajout | Message à copier |
| 13:31 | Limiter les choix client | Avant / après |
| 15:03 | Clés API, coûts mensuels, maintenance | Tableau de décision |
| 16:09 | Vérifier les noms/liens avant envoi | Checklist qualité |
| 17:55 | Demander les accès après cadrage | Pack démarrage |
| 18:25 | Cadrage validé + clés API = build | Gate avant développement |
| 18:37 | V1 en 4-5 jours maximum | Rythme de version |
| 20:17 | Présentation V1 + mail court | Pack V1 |
| 21:17 | Pour un projet à 8000 €, viser 3 modifications | Cadre des itérations |
| 21:57 | Fireflies à chaque call | Mémoire de call |
| 24:03 | Call 2, 3, 4 : garder toutes les transcriptions | Routine documentaire |
| 25:33 | Ne jamais corriger sans noter | Historique |
| 25:44 | Demander à Codex une checklist depuis un call | Prompt checklist |
| 26:42 | Protéger le périmètre | Évolutions futures |
| 27:26 | Ne pas parler technique, parler bénéfice client | Traduction technique -> valeur |
| 28:09 | Demander à Codex des screenshots via MCP | Preuve visuelle |
| 28:48 | Donner les retours à Codex comme tâches | Prompt V2 |
| 29:03 | Chaque tâche doit être testée en MCP | Contrôle qualité |
| 29:33 | Garder historique des décisions | Mémoire projet |
| 29:42 | Livrer avec guide d'utilisation | Livraison |
| 29:58 | La livraison est un moment commercial | Restitution finale |
| 30:21 | Proposer la suite après 4-5 jours d'usage | Upsell doux |
| 31:31 | Dossier présentation : audit, cadrage, V1, V2, V3 | Arborescence |
| 32:00 | Dossier call | Mémoire de réunions |
| 32:11 | Dossier projet | Fichiers de build |
| 33:42 | Structure légère pour gérer 10 projets | Conclusion |

## Prompts et messages à reprendre

### Prompt Codex - créer la présentation de cadrage

Ce prompt sert à transformer l'audit signé en page de cadrage GitHub claire.

```text
Comprends l'audit du client.
Le client a signé.

J'ai besoin que tu me fasses une nouvelle page GitHub pour la partie cadrage + planning.

Objectif :
- reprendre le design de la présentation d'audit
- expliquer le périmètre validé
- afficher le planning sur [DURÉE_DU_PROJET]
- préciser les accès à récupérer
- préciser ce qui est inclus et ce qui n'est pas inclus
- écrire de manière naturelle, claire et professionnelle

Contraintes :
- ne parle pas trop technique
- montre la valeur pour le client
- garde une structure simple à envoyer
- prépare une section "prochaine étape"

Résultat attendu :
- une page de cadrage publiable
- un mail court d'envoi au client
- une checklist interne avant de commencer le build
```

### Message - envoyer la V1

```text
Hello [PRENOM],

J'espère que tu vas bien.

J'ai terminé la V1. Tu peux la tester ici :
[LIEN_V1_TESTABLE]

Je t'ai aussi préparé une courte présentation pour comprendre ce qui a été fait, ce qu'il faut tester et les prochaines étapes :
[LIEN_PRESENTATION_V1]

Dis-moi ce que tu en penses.
Tu peux m'envoyer tes retours par mail, ou on peut se prendre un call court si c'est plus simple.
```

### Message - relance après V1

```text
Hello [PRENOM],

Je te relance sur la V1 envoyée [JOUR].

J'ai besoin de ton retour sur ces 3 points :
1. Est-ce que le parcours principal fonctionne comme tu l'imaginais ?
2. Est-ce que le ton / design / logique métier te convient ?
3. Est-ce qu'il y a un point bloquant avant que je prépare la V2 ?

Dès que j'ai ton retour, je transforme ça en checklist et je lance les corrections.
```

### Message - ajout hors périmètre

```text
Hello [PRENOM],

Oui, c'est possible.

Par contre, ce point n'était pas prévu dans le cadrage validé.
Pour le traiter proprement, j'estime environ [NOMBRE_JOURS] jours de travail.

Je peux te le proposer en ajout au projet pour [MONTANT] €.

Dis-moi si tu veux que je l'intègre maintenant, ou si tu préfères qu'on le garde dans les évolutions futures après la V1.
```

### Prompt Codex - transformer un call en checklist

```text
Tu es mon assistant projet-client.

Analyse la transcription de call ci-dessous.

MISSION
Transforme les retours du client en checklist actionnable pour la prochaine version.

Classe chaque point en :
- bug
- amélioration
- nouvelle demande
- question à clarifier
- règle métier à valider

Pour chaque point, donne :
- tâche claire
- priorité
- impact client
- preuve attendue
- risque si ce n'est pas traité

Important :
- ne mélange pas les demandes hors périmètre avec les corrections prévues
- garde les formulations client utiles
- prépare une section "à valider avec le client"

Transcription :
[COLLER_TRANSCRIPTION]
```

### Prompt Codex - corriger la V2 depuis les retours

```text
Tu es Codex, responsable de la V2.

Voici la checklist des retours client :
[COLLER_CHECKLIST]

MISSION
Traite les tâches une par une.

RÈGLES
- chaque tâche doit être corrigée dans le projet
- chaque tâche doit être testée
- si un test MCP / navigateur est possible, utilise-le
- ne traite pas les demandes hors périmètre sans les marquer comme "évolution future"
- garde une trace des fichiers modifiés
- prépare un résumé clair pour le client

SORTIE ATTENDUE
- tâches terminées
- tâches non traitées et raison
- tests réalisés
- captures ou preuves si disponibles
- message court pour envoyer la V2
```

### Message - proposer la suite sans forcer

```text
Hello [PRENOM],

Après quelques jours d'utilisation, je pense qu'on pourrait ajouter [IDEE_EVOLUTION].

Ce n'est pas urgent pour utiliser la V1, mais ça peut devenir intéressant si tu veux aller plus loin sur [BENEFICE_CLIENT].

Teste encore quelques jours et dis-moi si tu veux qu'on en parle.
```

## Les 23 tips à intégrer

1. Relancer tous les 3 jours.
2. Ne jamais disparaître.
3. Répondre en moins de 24 h.
4. Annoncer la prochaine étape.
5. Créer une présentation projet dès le début.
6. Reprendre le design de l'audit pour garder une expérience cohérente.
7. Cadrer ce que le client doit valider.
8. Limiter les choix du client.
9. Demander les accès dès le cadrage.
10. Ne pas perdre deux semaines pour des clés API.
11. Refacturer ou faire créer les comptes selon le niveau du client.
12. Faire une V1 en 4-5 jours maximum.
13. Viser une V1 testable, pas parfaite.
14. Transformer les retours en checklist.
15. Utiliser Fireflies à chaque call.
16. Ne jamais corriger sans noter.
17. Protéger le périmètre.
18. Classer bug, amélioration et nouvelle demande.
19. Ne pas parler technique au client.
20. Montrer l'avancement visuellement.
21. Tester chaque tâche en MCP quand c'est possible.
22. Livrer avec guide d'utilisation.
23. Organiser le dossier client pour pouvoir gérer plusieurs projets en parallèle.

## Structure de dossier recommandée

```text
[NOM_CLIENT]/
  presentation/
    audit/
    cadrage/
    v1/
    v2/
    v3/
  calls/
    call-01.md
    call-02.md
  projet/
    source/
    prompts/
    tests/
    livraison/
  decisions.md
  retours-client.md
  prochaines-actions.md
```
