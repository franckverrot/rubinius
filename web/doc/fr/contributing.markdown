---
layout: doc_fr
title: Contribuer
previous: Dépannage
previous_url: getting-started/troubleshooting
next: Communication
next_url: contributing/communication
---

Le projet Rubinius accueille avec plaisir vos contributions.
Il y a de nombreuses façons de nous aider.
Mais le plus important est que vous fassiez quelque chose qui vous intéresse :
c'est le meilleur moyen pour être enthousiaste et donner de l'énergie à votre travail.

Si vous avez des questions à propos de Rubinius, la meilleure méthode pour obtenir des réponses est
de discuter avec nous sur le canal IRC `#rubinius` sur [irc.freenode.net](irc://irc.freenode.net).

Voici quelques idées de ce que vous pouvez faire pour Rubinius.


## Exécuter votre code

Votre core est souvent plus vicieux que les specs... Exécutez votre projet favori avec Rubinius et
rapportez-nous les problèmes. Référez-vous à [Comment écrire un ticket](/doc/fr/how-to/write-a-ticket).


## Demandez de l'aide

Tout ce que nous pouvons faire pour vous aider, nous le ferons.
Assurez-vous d'effectuer votre propre investigation aussi, si possible.
Rubinius essaie d'être un projet que vous pouvez étudier facilement, qui est didactique
et que vous pouvez même étendre, nous l'espérons.

Nous accepterons certainement et apprécierons de simples rapports de bogues, mais nous pouvons donner
une priorité aux tickets qui incluent des étapes simples de reproduction du problème.
Encore meilleurs sont les tickets qui incluent des RubySpecs qui démontrent le bogue
et un patch qui le résout.


## Ecrire des specs

  1. Exécutez `bin/mspec tag --list incomplete <dir>` pour afficher les specs qui ont été
     tagguées incomplètes.
     Ces specs peuvent nécessiter une simple revue, ou être incomplètes/manquantes pour
     une classe en particulier.

     NOTE: Vous pouvez spécifier un pseudo-répertoire `:files` pour `<dir>`, qui
     affichera les tags pour toutes les specs qui devraient passer sous Rubinius.
     Ou vous pouvez spécifier tout sous-répertoire du répertoire `spec/` pour
     lister les tags des specs dans ce sous-répertoire.

  2. Trouvez les comportement non spécifiés. Lisez
     [Comment écrire un Test Ruby](/doc/fr/how-to/write-a-ruby-spec).


## Fix Failing Specs

  1. Run `bin/mspec tag --list fails <dir>` to show specs tagged as failing.

     NOTE: You can specify the pseudo-directory ':files' for \<dir\>, which will
     show tags for all the specs that should run on Rubinius. Or you can
     specify any subdirectory of the spec/ directory to list tags for specs in
     that subdirectory.

  2. Pick a spec that looks interesting and see if you can write a patch that
     will make it pass.


## Write Docs

Study how Rubinius works and write highlevel documentation that will help
others learn about the implementation details.


## Cleanup Code

Review the [Style Guide](/doc/en/contributing/style-guide/) for coding
guidelines.


## Triage Tickets

  * Revive or close old tickets.
  * Build minimal test cases that reproduce the bugs. Then see if there are
    already RubySpecs for the issue. If not, consider writing some.
