# La dataviz en JavaScript

## Pourquoi (ne pas) utiliser les outils existants

Je voulais vraiment parler de toutes les différentes technos standards pour faire du rendu graphique dans le navigateur avec JavaScript. Le truc, c'est qu'il y a d'excellentes raisons d'utiliser les outils existants, que ça soit des moteurs de rendu comme Pixi.js ou Raphael.js pour des questions de compatibilité, ou encore des bibliothèques dédiées à la dataviz comme sigma.js ou d3.js pour ne pas avoir à gérer soit-même des choses difficiles.

Du coup, je savais pas trop comment introduire cette présentation. Jusqu'à la semaine dernière, avec un post du blog Sam&Max qui trash complètement JavaScript. Personnellement, j'aime beaucoup l'environnement parisien des techs meetups où les gens viennent présenter ce qu'ils aiment dans leur métier et les technos qu'ils manipulent au quotidien. Mais là, c'était tout l'inverse.

Lien:
http://sametmax.com/un-gros-troll-de-plus-sur-javacscript

Du coup je lis ça et je lis les commentaires pour voir ce que les gens pensent de posts comme celui-ci. Et je tombe sur un super commentaire de Olivier Penhoat, qui dis ça:

"En réalité, JavaScript est un langage exigeant faussement facile qui nécessite d’aimer le bricolage, l’artisanat."

Et c'est la principale raison qui me pousse à essayer de tout faire moi-même: Le JavaScript ça m'éclate. Composer avec toutes les possibités de l'API du navigateur pour faire mes rendus de la meilleure manière, ça permet de progresser et de faire des visualisations qui sont de mieux en mieux avec le temps.

Bref, même si dans certains projets, pour diverses raisons, je dois utiliser des outils externes pour développer mes visualisations ou applications, je m'éclate toujours beaucoup plus en travaillant directement avec les APIs natives.

## Le vif du sujet

J'ai commencé à développer il y a quelques années en école d'ingé, et je dois reconnaîtren que ça ne me fascinait absolument pas, sur le coup. J'avais envie de faire des trucs, mais je savais pas quoi. A ce moment là, je trainais avec les gars du projet Gephi, et assez vite, il fallait que quelqu'un développe une solution pour pouvoir visualiser des graphes sur le Web. Et du coup, j'ai commencé à bosser avec Flash et AS3.

A ce moment là, je n'ai encore jamais développé quoique ça soit qui affiche autre chose que du texte dans une console, et le premier contact était chouette:

var c:Sprite = new Sprite();
c.graphics.beginFill(0x666666);
c.graphics.drawCircle(100, 100, 50);
c.graphics.endFill();
parent.addChild(c);

Et là, la magie opère: Le rond apparaît à l'écran. Mais c'est encore plus fort! Flash propose un arbre graphique dans lequel on peut mettre des Sprites, sur lesquels on peut dessiner ce que l'on veut. Et malgré ça, Flash gère parfaitement le rollover.
