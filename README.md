# Notes datées

Journal chronologique de réflexions et de thèses (principalement d'investissement), publiées et horodatées sans recherche d'audience. Chaque article est daté à sa publication et n'est jamais retouché après coup — les mises à jour vont en addenda, datées séparément.

## Mise en ligne (5 minutes)

1. Crée un nouveau repo GitHub, public, nommé exactement `<ton-pseudo-github>.github.io`
   (ex : si ton compte GitHub s'appelle `christophedelaplace`, le repo doit s'appeler `christophedelaplace.github.io`)
2. Pousse tout le contenu de ce dossier dans ce repo (branche `main`)
3. Va dans **Settings → Pages** du repo, vérifie que la source est bien la branche `main`, racine `/`
4. Le site sera accessible sous quelques minutes à `https://<ton-pseudo-github>.github.io`

Pas besoin d'installer Jekyll en local : GitHub Pages le fait automatiquement au moment du push (thème `minima`, déjà configuré dans `_config.yml`).

## Publier un nouvel article

Crée un fichier dans `_posts/` nommé `AAAA-MM-JJ-titre-court.md`, avec cet en-tête :

```
---
layout: post
title: "Titre de l'article"
date: AAAA-MM-JJ 00:00:00 +0200
---
```

Le nom de fichier ET le champ `date` doivent correspondre à la date réelle de publication — c'est ce qui donne, avec l'horodatage du commit Git, la double preuve d'antériorité.

## Après le premier push

Retourne dans `_posts/2026-09-14-these-ams-osram.md`, récupère l'URL du commit (bouton "History" sur GitHub, ou l'URL du commit affichée après le push), et colle-la dans le champ prévu en haut de l'article ("Preuve d'antériorité : ..."). Ce lien pointe vers une version figée du fichier, horodatée par GitHub, que personne — toi y compris — ne peut modifier rétroactivement.

## Personnaliser (optionnel, plus tard)

- `_config.yml` : titre, description
- Domaine personnalisé : possible via un fichier `CNAME`, si tu veux un jour `tonnom.com` plutôt que `tonpseudo.github.io`
