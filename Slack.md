L'incubateur utilise [Slack](http://startups-detat.slack.com/) comme service de messagerie instantanée.

## S'inscrire

- **Avec une adresse email en `@beta.gouv.fr` :** aller sur http://startups-detat.slack.com/ et se créer un compte.
- **Avec n'importe quel autre email :** demander à @MattiSG, par exemple.

## Conventions de nommage des canaux

### Préfixes

Pour améliorer la découvrabilité, chaque canal est préfixé d'une catégorie.

- `startup-` : canaux liés à des produits.
- `api-` : canaux liés à des API.
- `incubateur-` : canaux d'organisation interne à l'Incubateur.
- `etalab-` : canaux d'organisation interne à Étalab.
- `bureaux-` : canaux liés à des espaces physiques.
- `bruit-` : canaux de discussion sans but productif.
- `domaine-` : canaux de discussion liés à des pratiques / compétences.
- `tmp-` : canaux liés à un événement ponctuel et destinés à être archivés rapidement.

### Doubles canaux des Startups

Les canaux de startups sont préfixés par `startup-`. Lorsqu'ils atteignent un haut volume, un second canal est créé, du même nom suffixé par `-info`. Les membres intéressés par l'évolution du produit mais pas par ses changements quotidiens peuvent ainsi échanger sur un canal à faible volume.

> Cela correspond plus à la croissance d'une startup que l'ancienne organisation qui suffixait le canal à fort volume par `-internals`.

### Nommage

Les préfixes et suffixes sont séparés par des `-`. Les noms de base sont joints par des `_`.

_Voir https://github.com/sgmap/beta.wip/pull/1 pour tout l'historique de ces conventions._

## Commandes

Plusieurs commandes « slash » sont disponibles pour nous faciliter la vie. Ces commandes sont activées en écrivant un message commençant par une barre oblique (`/`).

### `/trad`

Comprendre et documenter les acronymes administratifs étranges. N'hésite pas à enrichir ce glossaire partagé au fur et à mesure de tes découvertes :wink:

Exemple :

> - j'ai vu la DGA de la DGFIP au SIDSIC
> - /trad SIDSIC
> - _bot :_ SIDSIC : Service interministériel départemental et systèmes d’information et de communication

_Le bot glossaire de Slack est une instance de [`glossary-bot`](https://github.com/codeforamerica/glossary-bot) hébergée sur Heroku (id : `glossaire-betagouvfr`) sur le compte de @MattiSG._

### `/compte`

Créer un compte mail pour les nouveaux et nouvelles.

À utiliser de préférence dans le canal [🔒`#incubateur-secretaria`](https://startups-detat.slack.com/messages/incubateur-secretaria/). Syntaxe :

```
/compte prenom.nom [*]adresse@mail.com password
```

- `prenom.nom` est l'identifiant correspondant à une fiche personnelle _déjà publiée sur beta.gouv.fr_ ;
- `adresse@mail.com` est l'adresse à laquelle on notifiera la création du compte, et vers laquelle les mails seront redirigés (cette redirection est optionnelle et peut être inhibée en ajoutant une étoile devant l'adresse) ;
- `password` est le mot de passe que la personne concernée vous aura soufflé à l'oreille. Ce mot de passe ne sera pas affiché sur le canal Slack.

_Commande implémentée par [`betaGouvBot`](https://github.com/sgmap/betaGouvBot) et hébergée sur le Heroku de l'Incubateur._

### `/badge`

Demander l'édition d'un badge pour l'accès aux [[locaux]] de Mirabeau.

À utiliser de préférence dans le canal [🔒`#incubateur-secretaria`](https://startups-detat.slack.com/messages/incubateur-secretaria/). Syntaxe :

```
/badge prenom.nom
```

où `prenom.nom` est l'identifiant correspondant à une fiche personnelle *déjà publiée sur beta.gouv.fr*.

_Commande implémentée par [`betaGouvBot`](https://github.com/sgmap/betaGouvBot) hébergée sur le Heroku de l'Incubateur._


## Conventions emojis

### 🚀 : succès !

Pour partager une avancée, un succès ou une release avec le reste de l'incubateur, postez un petit message dans [🔒`#incubateur-annonces`](https://startups-detat.slack.com/messages/incubateur-annonces) – en ajoutant une `:rocket:` 🚀 au début du texte.

Pas besoin d’être bien long ; c'est juste pour signaler aux autres ce dont vous êtes heureux ou fier (et pour recueillir les applaudissements).

Par exemple :

> - 🚀 _Les utilisateurs du site peuvent enfin modifier leur adresse email de contact._
> - 🚀 _On a sorti OpenFisca 9, avec la nouvelle version de l’API web et les données du RSI_
> - 🚀 _Nos affiches sont visibles dans le métro depuis ce matin !_
> - 🚀 _C’est confirmé, Eva nous rejoindra en mars comme data-scientist_

Évidemment ne pas hésiter à rajouter ensuite un lien, une photo, une capture d'écran, un gif animé, etc.

Pour recevoir une notification de Slack à chaque "🚀", vous pouvez également rajouter `:rocket:` dans votre [liste des mots-clefs](https://get.slack.help/hc/fr-fr/articles/201398467-Notifications-des-mots-cl%C3%A9s).

_Cette convention est encore neuve, et en cours d'expérimentation (avril 2017).<br>
Plus de détails [par ici](http://kemenaran.winosx.com/posts/partager-les-succes/)._

### 💩 : négativité inutile.

Pour faire remarquer qu’un message peut être interprété comme particulièrement négatif, voire qu’il serait dommageable pour le collectif que ce qui a été écrit soit cité, une réaction par 💩 permet de signaler à son auteur qu’on se sent mal à l’aise avec le texte. Il s’agit d'une évaluation personnelle, et l'usage recommandé en est la réaction, afin de ne pas détourner la conversation sur le fond mais de suggérer une amélioration de la forme.

Par exemple :

> les informaticiens de la DRFTAPS sont vraiment des abrutis, ils ont encore réussi à planter le serveur de leur API, ÇA ME SAOULE
> +💩
>
> → le serveur de l'API de la DRFTAPS est encore en rade, ÇA ME SAOULE _(edited)_
