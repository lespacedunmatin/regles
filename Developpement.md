Contraintes du développement logiciel
=====================================

## Langue

### Code

Par uniformité avec les bibliothèques standard fournies par les langages de programmation, les objets (méthode, fonctions, variables…) manipulés dans le code seront nommés en anglais.

> Exemples : `getCurrentYear()`, `var total = sum(1, 2)`.

En application des principes du [<abbr title="Domain-Driven Design">DDD</abbr>](http://blog.infosaurus.fr/post/2009/10/13/DDD-Vite-Fait,-les-fondamentaux-de-DDD) et des bonnes pratiques de programmation, les éléments du domaine métier conservent leur nom intact, y compris dans le code, et sans traduction s’ils sont en français.

> Exemples : `getRevenuFiscal()`, `var total = sum(chefDeFamille, conjoint)`.

### Backlog

Par souci de lisibilité pour les partenaires, notamment administratifs, la langue utilisée pour la description et le suivi de fonctionnalités est le français.

### Discussions

En revanche, pour éviter le coût du changement de contexte, les discussions techniques, notamment par le biais de commentaires ou d'échanges par des logiciels spécialisés, peuvent se faire en anglais, la langue la plus utilisée dans le cadre du développement logiciel.

### Documentation

Attention à ne pas rédiger un `README` _intégralement_ en anglais. Un simple résumé en français _([exemple](https://github.com/sgmap/paie-api#readme))_ vous permettra de [respecter la loi](https://www.legifrance.gouv.fr/affichTexte.do?cidTexte=LEGITEXT000005616341&dateTexte=vig#LEGIARTI000006421216).


## Infrastructure / langages

Fais ce que tu veux. Mais prévois que tu ne seras probablement pas le seul à intervenir sur ton produit… s'il marche  :wink:


## Usage de services commerciaux externes

Un service commercial externe est un outil ou un composant logiciel sur lequel la DINSIC n'a pas tout à la fois :

- la liberté d'utiliser le logiciel ;
- la liberté de copier le logiciel ;
- la liberté d'étudier le logiciel ;
- la liberté de modifier le logiciel et de redistribuer les versions modifiées.

> Il s'agit des quatre libertés fondamentales du [logiciel libre](https://www.gnu.org/philosophy/free-sw.fr.html).
>
> Cela n'implique pas nécessairement qu'il s'agisse d'un logiciel libre. Un logiciel sous propriété intellectuelle DINSIC peut ainsi respecter ces critères.


### Éviter si critique

Un outil ou composant logiciel dont une défaillance empêche le produit de remplir une promesse faite à l'utilisateur **ne devrait pas** être un service commercial externe.

> Le logiciel doit pouvoir être réutilisé par d'autres acteurs que la DINSIC… et si un composant critique disparaît, on est coincés !
>
> Exemples :
>
> - Framework applicatif.
> - Serveur.
> - Composant de compilation.
> - Moteur de recherche.


### Utilisable si optionnel

Un outil ou composant logiciel qui n'est pas nécessaire pour que le produit tienne les promesses faites à l'utilisateur est dit « support ». Les outils supports à la production **peuvent** être des services commerciaux externes.

> Exemples :
>
> - Outil de suivi d'avancement.
> - Outil de déploiement continu.
> - Composant de suivi d'usage.


## Licence

Voir [[comment publier | Publier ]].
