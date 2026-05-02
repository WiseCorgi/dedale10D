+++
title = 'Mise_en_ligne'
date = 2026-05-02T01:58:06+02:00
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = "Arnaud"
authorTwitter = "" #do not include @
tags = ["", ""]
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
+++

# Mettre en place un blog avec Hugo

Je suis parti d’un objectif simple : créer un blog personnel pour documenter mon apprentissage.

Le choix s’est porté sur Hugo, principalement pour sa rapidité et sa structure statique. L’idée était de garder quelque chose de simple, mais suffisamment flexible pour évoluer. Et à moindre coûts..

## Mise en place initiale

Le projet a commencé par une installation locale de Hugo. J’ai ensuite créé un dépôt GitHub pour versionner le projet et un compte Cloudflare pour l’hébergement.

L’objectif était d’avoir un flux simple :
Hugo en local, GitHub comme source, Cloudflare pour la mise en ligne.

## Premier thème et premières difficultés

J’ai commencé avec un thème appelé Terminal. L’installation semblait simple, mais rapidement des problèmes sont apparus lors du déploiement.

Le blocage principal venait de la gestion des submodules Git. Le thème était intégré comme submodule, ce qui a provoqué des erreurs lors du build sur Cloudflare.

Les erreurs n’étaient pas immédiatement lisibles, mais elles empêchaient le site de se déployer correctement.

## Nettoyage et changement de direction

Lasse de tourner en rond avec le thème Terminal, j'ai préféré changer complètement en passant à PaperMod et de faire un nettoyage complet :
suppression des anciens layouts, des configurations héritées et des traces de submodules Git.

## Mise en place de PaperMod

Le nouveau thème a été installé manuellement. La configuration a été simplifiée et les sections du site ont été structurées en deux parties principales : carnet et projets.

Cela a permis d’avoir une base claire, sans surcharge technique.

## Résolution des erreurs Hugo

Plusieurs erreurs sont apparues lors des tests locaux.

La plupart venaient de deux sources :
des fichiers hérités de l’ancien thème et des erreurs dans les fichiers Markdown.

En corrigeant la structure et en supprimant les éléments inutiles, le site a fini par fonctionner correctement en local.

## Mise à jour de l’environnement

Hugo a été mis à jour vers une version plus récente en mode extended. L’installation a été faite manuellement pour éviter les gestionnaires de paquets automatiques.

Cela a permis d’assurer une meilleure compatibilité avec PaperMod.

## Mise en ligne

Le projet a ensuite été connecté à GitHub et Cloudflare Pages.

Une erreur persistante liée aux submodules a nécessité un nettoyage complet du dépôt Git. Une fois corrigé, le déploiement a pu fonctionner correctement.

## Conclusion

Le projet est maintenant fonctionnel, mais pour un néophyte comme moi, je doit avouer que cela n'a pas été si evident. Pour le moment ça à l'aide de rouler, et cela devrait me suffir 

Le blog tourne en local et est prêt pour une mise en ligne stable via Cloudflare. La prochaine étape consiste à passer de l’authentification Git HTTPS vers SSH afin de simplifier la gestion du dépôt.
