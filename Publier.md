Comment mettre nos productions à disposition du public
======================================================

Licence
-------

Sauf demande expresse justifiée et discutée en interne, notre code est publié sous licence libre. Une licence [AGPL-3.0](http://www.gnu.org/licenses/agpl-3.0.fr.html) est une bonne valeur par défaut.

### Compatibilité

Attention, si vous incluez du code externe dans le vôtre (pas du lien, mais bien de la copie), à n'inclure que du code sous une licence compatible avec la licence AGPL.

Si vous utilisez des bibliothèques non compatibles AGPL, pensez à le [préciser dans la licence](http://www.gnu.org/licenses/gpl-faq.html#GPLIncompatibleLibs) avant la phase de passation.

### Appliquer une licence

Inclure le fichier de licence [au format texte brut](http://www.gnu.org/licenses/agpl-3.0.txt) à la racine du dépôt concerné, sous le titre `LICENSE.AGPL.txt`.

> Ce nom en améliore la découvrabilité.

Si vous travaillez sur un module NPM, pensez à ajouter la propriété `"license": "AGPL-3.0"` dans votre `package.json`.


Vocabulaire
-----------

### Handicap

On parle de personne « en situation de [handicap](http://www.legifrance.gouv.fr/affichCodeArticle.do?cidTexte=LEGITEXT000006074069&idArticle=LEGIARTI000006796446) » et non de personne « handicapée ».

> Je la classais volontiers parmi la foule des expressions issues du politiquement correct, pensant qu’elle voulait parler des handicapés mais en arrondissant les angles. Je n’ai pas tout de suite compris qu’elle ne désignait pas uniquement les personnes atteintes d’un handicap permanent, mais élargissait la notion de handicap à tout individu pouvant éprouver une difficulté à accomplir une tâche dans un contexte donné.

[Source](http://tanguyreve.unblog.fr/2012/05/03/personne-handicapee-ou-personne-en-situation-de-handicap/).


Syntaxe
-------

### Écriture épicène

Nos outils s'adressent à tou·te·s les citoyen·ne·s, mais la langue française impose souvent de faire des choix de genre (féminin ou masculin), avec une préférence pour le masculin « qui l'emporte » dans un groupe.

Pour éviter de genrer les outils et les rendre ainsi plus inclusifs, construisez des phrases **neutres en genre**.

Vous pouvez par exemple expliciter le sujet, en utilisant des termes génériques ([épicènes](https://fr.wikipedia.org/wiki/Épicène)) tels que « personne ».

En désespoir de cause, faites apparaître les formulations masculines et féminines dans la même phrase, comme le classique « né(e) en ».
Cependant, pour fluidifier la lecture, plutôt que des parenthèses, utilisez le [point médian](https://fr.wikipedia.org/wiki/Point_médian#Utilisation_dans_le_langage_non_sexiste) : `·` (`U+00B7`, raccourci sous macOS : `⎇⇧F`).

> Pour en savoir plus, le [Haut Conseil à l’Égalité entre les femmes et les hommes](http://www.haut-conseil-egalite.gouv.fr/) a élaboré un [Guide pratique pour une communication publique sans stéréotype de sexe](http://www.haut-conseil-egalite.gouv.fr/IMG/pdf/hcefh__guide_pratique_com_sans_stereo-_vf-_2015_11_05.pdf).


Typographie
-----------

### Guillemets

Les guillemets français sont [`«`](http://unicode-table.com/fr/00AB/) et [`»`](http://unicode-table.com/fr/00BB/), avec des espaces insécables [` `](http://unicode-table.com/fr/00A0/) (raccourci sous macOS : `⎇⇧ `). respectivement après et avant le guillemet.

[Plus d'informations](https://www.noslangues-ourlanguages.gc.ca/bien-well/fra-eng/ponctuation-punctuation/guillemets-quotation-fra.html).

### Points de suspension

Les points de suspension sont [`…`](http://unicode-table.com/fr/2026/) et non `...` (trois points). Cette distinction est importante pour les sauts de ligne, les lecteurs d'écran et le copier-coller.


Suivi d'usage (_analytics_)
---------------------------

Toutes les statistiques d'usage des produits web sont disponibles sur l'instance [Piwik](https://piwik.org) publique [`stats.data.gouv.fr`](https://stats.data.gouv.fr). Cette transparence est importante pour incarner notre démarche d'ouverture et de collaboration avec les citoyens.

> Pour ne pas gonfler artificiellement ces statistiques, les IP suivantes peuvent être exclues dans Piwik :
>
> - `185.24.184.74` (Mirabeau)
> - `46.218.59.235` (ADSL Sully)
> - `89.225.241.174` (fibre Sully)
> - `46.218.46.150` (Mutinerie)
