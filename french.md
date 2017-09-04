    Introduction
L'emotilang est un langage construit permettant de representer un ensemble
complexe d'emotions par des symboles simples et une grammaire complexe formant
des "mots" ressemblant à des émoticons que l'on appelle sémioticons... 
Okay, c'était totalement pompeux, pour l'instant on est 5 à l'utiliser et 
"on", c'est deux de ces cinq personnes qui viennent de trouver ce mot.
Enfin bref.
Tout ca pour dire, ce petit carnet que je te prete à lire est ici le
récapitulatif de cette langue jusque là.

Quelle est l'interêt d'une telle langue? Eh bien, le language modèle ce que
l'on dit, et je me disais que c'était interessant d'avoir un langage pour
transferrer _uniquement_ les émotions et non le contexte. Ce langage décrit
donc uniquement ce qui est présent en soi au moment où l'on parle et
l'évolutions de ces sentiments
 J'expliquerais à la fin certains choix de design, et les suggestions proposés.
Il est bien entendu évident que n'importe qui, toi compris donc, peut le
modifier à sa guise pour rajouter des choses et des complexions, des
expletions qui viendrait à manquer.
J'apprecie d'ailleurs beaucoup les feedbacks, donc n'hésite pas à me dire les
modifications utiles que tu y vois, ou y a apporté!
Dernier petit point: C'est apparament plus simple de commencer en s'habituant
aux symboles, puis ensuite de structurer le tout par la grammaire. Je dis ca
si jamais elle te semblerait trop lourde a digerer

^(%_[$]0&) `.:.`!

    Vocabulaire
    Intensifieur
~ Faible intensite
! Forte intensite
= Intensite similaire

    Emotions
~ Deception, soulagement (Attenuation du sentiment)
! Entousiasme, excitation, hate (Accentuation du sentiment)
= Indifference, ennui, excitation (Egalite du sentiment)
@ Colère
# Peur, appréhension
$ Fierté, satisfaction
% Désir, envie
^ Joie
& Envie de creer, partager, curiosité
* Surprise, étonnement
0 Integration à l'univers, l'instant présent
1 Integration à soi, l'instant présent
6 Amusement, playfullness
v Éspoir
\/ Gène
? Confusion
. Réflexion
, Vide
<> Frustation, impuissance
; Tristesse
x Haine (de soi, du monde), folie 
3 Unmet need, manque
4 Douleur (physique), souffrance
: Compréhension
- Fatigue
_ Serenité, accalmie
+ Remords, culpabilité
ç Admiration, passion
() Concentration
` Empathie

     Groupe:
() Je me concentre sur ces sentiments
[] J'essaye de me distantier de ces sentiments
{} J'essaye d'embraser ces sentiments
`` Par rapport a des sentiments d'autres personnes
'' Ces sentiments se suivent les uns apres les autres en boucle (lire de gauche a droite)
"" Desambiguation (Ca ne change rien gramaticallement, il faut les lire a part)
| Repetition du symbole matché parce que flemme de le reécrire.

   Combinaisons courrantes:
%> Envie frustré
*ç* Admiration
:3 envie de comprendre
/3= Stress

	Grammaire
Les semioticons se lisent de l'exterieur vers l'interieur, la plupart du
temps, les symboles de part et d'autre sont les mêmes, et signifie qu'ils
entourent l'emotion au centre, qu'au centre se trouve...
Comme suit:

 ^_^ (Joie entourant le calme, calme au centre de la joie)
 >< (Frustration)
 .:. (Je reflechis et au centre se trouve la compréhension)

Si les symboles ne se correspondent pas, cela veut dire qu'il y a eu
transformation: L'émotion de base s'est transformé en la suivante par
l'intermediaire de ce qui est au centre

 ^.# (Je suis joyeux, mais cette joie se transforme en apprehension après reflexion)
 ;#@#v (Je suis triste, j'ai peur et je suis en colère, mais ma tristesse se transforme en espoir)

On peut avoir besoin de transformer tout un groupe en tout un autre.
La plupart du temps, ce n'est pas ambigue et un simple espace suffit

 ,_, ^_^ (Le calme du vide se tranforme en calme de joie)
 >@> ;v; (La frustation avec colère se transforme en tristesse avec espoir)

Néanmoins, si l'on a peur que ce soit trop ambigüe ou que la lecture en est
trop dure, on peut echapper le premier groupe pour dire qu'il ne s'agit que
d'une seule émotions.
Les émotions précedentes sont alors:

",_," ^_^
">@>" ;v;

NB: Il est à noter qu'il n'y a pas besoin de guillemets sur le second groupe,
vu que ce n'est pas ambigüe.

Autre symbole changeant le sens: Les appostrophes.
Quand on rencontre celles-ci, on lit tout ce qui se trouve à l'interieur de
gauche à droite. Ca veut dire que les émotions arrivent les unes à la suite
des autres, en boucle.

  ';^!=<' (Tristesse puis joie, enervement et frustration)
  '?.:'  (Remise en doute, joie puis comprehension: Processus de reflexion)

Si tu as lu un peu les symboles, tu t'etonnera sans doute de la grande
polyvalence de ~, ! et =. C'est normal: Ce sont des intensifieurs.
Tout symbole de "gramaire" a vocation a aussi avoir un sens seul, c'est
pourquoi leur but est double:
Si un intensifieur est face a un autre, il indique une progression de
l'emotion décrite:

  !'4+'~ (La grande douleur suivi du remords s'en vont en diminuant jusqu'a s'éteindre)
  !^6^! (Forte joie entourant un amusement, une taquinerie)

Mais parfois ils peuvent eux meme etre une emotion. Leur sens est dependant
du contexte, ~ indique une diminution de l'émotion, dans un contexte heureux
ca peut etre du soulagement, mais dans un triste de la déception.

 ^~^ (Soulagement)
 #><! (Peur, au centre la frustration, la peur se transforme en une forme d'impatience)

Ça peut sembler bizzare, mais on s'y fait vite
On peut échapper les intensifieurs par des guillemets pour dire qu'il faut les
prendre comme émotions:

  !^"!"^! (Forte joie teintée d'excitation)

Deux dernière règles de grammaire:
Normalement un signe qui entoure une emotion ne doit reaparaitre a l'interieur
de cette émotion que si celle ci contient un groupe pour l'échapper
Néanmoins, une règle un peu speciale changent cela: Si l'on repete un
ensemble de symbole élementaires, cela veut dire que ces émotions sont
entremeles:
  
 0:0: Comprehension du Logos
 _~_~ Calme et soulagement

On peut bien sur mettre des choses à l'interieur de ces émotions:

 0:$:0 Acces a l'univers, au centre se trouve la satisfaction
 _~(.?.)_~ Calme et soulagment, au centre se trouve la reflexion, le doute

Si les émotions sont plus complexes on peut se retrouver en face du problème
de lourdeur. Par exemple:

^%^ ">/<" ^%^ (De la joie avec envie avec de frustration/gène au centre)

Il peut être lourd de devoir réecrire le dernier smiley, surtout si celui-ci
est très complexe.
On introduit alors une nouvelle notation qui ne change pas le sens: les barres
|
Celles ci indiques qu'il faut repeter l'émotion à laquelle elle correspond et
sont en faces de.
Le sémioticons ci-dessus s'écrit donc aussi

"^%^" >/<  |

Il est a noter que cela induit une confusion: est-ce que "^%^" >/< _ || veut
dire ^%^ >/< _ >/< ^%^ ou ^%^ >/< _ ^%^ >/<
Le sens ne change que peut (est-ce que les émotions sont entrelacées ou
sont-elles imbriquées), mais la difference est à noter.
La convention est alors de mettre les deux barres du même côté si l'on veut
les imbriquer (le premier), et en alternes comme suit ^%^ | _ >/< | si l'on
veut les entrelacer (le second)

Dernier petit point, si on veut lier des sentiment par des "et", on repete l'emotion inchangé alentour:
 ^6^&^ (Joie entourant de l'amusement et de la curiosité)
 +;+=+ (Regret entourant de la tristesse et de l'indifference)

Enfin (oui j'ai menti en disant que ce serait fini), petite désambiguation par
rapport aux groupes:
``, (), [] et {} groupent tout quatres les émotions differement (il n'y a
donc pas besoin de mettre de guillemets autour)
`` s'utilisent quand l'on prend le sentiment d'une autre personne, qu'on le
ressent
() quand l'on parle par rapport a des sentiments, qu'on se concentrent sur les
siens
[], on essaye de les repousser, {} de les embrasser.

[@>@] {0_`_0} (Je repousse la colère et la frustration pour accepter
l'integration, le calme et l'écoute)
?()? (Je suis confus/e par rapport à mes sentiments)
>`@#@`/ (Je me sens frustrée, genée par les sentiments de colère et de haine que je ressens de leur part) 

   Suggestions et pseudo FAQ:
Bien sur, par FAQ, j'entends plus les choix que l'on a souvent du aborder
ensemble.

  La grammaire très complexe
La grammaire peut sembler arbitraire, comme les symboles. Pourquoi reproduire
de l'autre côtés? Pourquoi autant de règles? Pourquoi ^ veut dire la joie?
Pour le choix des symboles, j'ai choisi d'utiliser des symboles qui
permettraient de se reconnaitre simplement dans des smileys simples, qu'ils se
rapprochent des smileys typiquement employés comme ^^ par exemple.
Les règles de symmetrie vont dans ce sens, celui esthetique notamment (et
égallement, cela permet d'avoir une lecture globale rapide)
Enfin, la complexité des règles permettent de se rapprocher de la complexité
des sentiments. Peut-être que certainnes sont superflues, elles se feront
alors oublier avec le temps.

  L'imprecision des symboles
Les symboles pourrait te sembler très imprécis: Fierté et satisfaction,
culpabilité et remords... 
En fait, il s'avère qu'un point qui me semblait
important dans ce langage, c'est la distinction entre les pensées et les sentiments.
L'emotilang n'est pas faite pour exprimmer ce que l'on pense (il y a le
français ou n'importe quelle langue pour ça), mais ce que l'on ressent. Par la
même, il m'a semblé important de les differencie, de ne regroupper ensemble
uniquement par la sensation qu'elle provoque et pas par la situation.
Égallement d'éviter une certaine dichotomie entre les "bons" sentiments" et
les mauvais
Une petite liste des émotions qui sont associés les plus contestés

	Culpabilité <=> Remord
Sans doute que je vais finir par l'integrer vu combien tout le monde semble
dire que ce n'est pas pareil. Une grande difficultés pour les differencier, est
que l'on n'arrive pas à décrire le sentiment sans parler des situations dans
lesquels ils surviennent.
Égallement, à chaque fois que l'on décrivait culpabilité, on utilisait des
notions de bien et de mal qui sont des pensées.
Le plus proche que j'ai réussi à avoir, c'est qu'il y a dans culpabilité une
notion d'empathie envers la souffrance de l'autre (mais dans ce cas, ne peut
on pas l'expliciter?)

	Cuteness <=> Admiration
Voir la proposition dans les émotions manquantes, c'est apparament trop
ambigue et je suis d'accord

  Le manque de contexte
Par choix de design, comme je disais l'emotilangue ne décrit pas le
contexte mais simplement les émotions ressentis.
Néanmoins, cela pose un problème quand les émotions sont dirigés vers un objet
du contexte (Je veux une glace par exemple), et encore pire si les émotions
sont orientés differement sur plusieurs objets.
Jusque là j'employais plusieurs phrase accompagnés de leur smiley, mais peut
être que ce serait interessant de se pencher dessus?

  Les besoins et envie physiques
Pour l'instant, seul - exprimme quelque chose de l'ordre du corps (although il
exprimme plus un trop plein ou un manque d'ennergie), mais il n'y a pas de 
symboles pour la libido ou la faim par exemple. 
On se demandait si cela était pertinenent.
Si ça l'est, peut être faut il distinguer les états des émotions et que les
états aient leur symboles à eux?
Une solution simple serait un groupe qui indique que les émotions suivantes
font refference au corps, par exemple en mettant un m de chaque côté
Si ça ne l'est pas, On pourrait exprimmer la libido par % ou >%! (Envie, ou
envie qui se transforme en impatience) et la faim par > ou 4 en fonction de
l'intensité (frustration ou douleur)
J'aime bien la solution du m, à voir.

  Le manque de négations 
Le manque de négations est volontaire dans la même lignée, il est plus
interessant de décrire ce que l'on ressent que ce que l'on ne ressent pas.
Néanmoins, ~ permet de marquer lorsqu'un sentiment est faible ou s'en va
faiblissant, et [] si on en est l'acteur.
  
  Les intensifieurs
Les intensifieurs étant ambigu, il est possible qu'on les fasse disparaitre
par la suite en tant qu'emotions. Il ne marquerait alors plus que des
variations de l'intensité de l'émotion

	! et = ont l'ennuie et l'impatience en commun
L'idée de base, c'est que ce n'était pas égallement la même chose. = est une
sorte de "et rien ne change" tandis que "!" est une sorte d'impatience, qui
contrairement à = devient trop forte, genre je tiens plus en place.

  Sentiments sur les sentiments
Je réflechis à une syntaxe du type (-)^ : Je suis content par rapport à ma
fatigue.
Elle me semblerait très cohérente, mais je ne sais pas si elle apporterait
beaucoup.
Mais surtout, je reflechis à certains symboles qui serait toujours en rapport
aux sentiments exprimés, comme 3 l'unmet need par exemple. On pourrait alors
désambiguer par des guillemets?
Que voudrais dire -(^) aussi? Je suis fatigué et me concentre sur ma joie?
Auquel cas l'on perd le sens gramatical.
Enfin, certains symboles comme > et \ ont deux sens d'écritures differents, peut être
pourrait on utiliser cela 

  Indiquer où l'on se trouve par rapport à ces sentiments
Jusque là, on considère que l'émotion au centre est la où c'est le plus
présent, mais ça manque de précision.
Sur papier on peut mettre en gras pour indiquer où l'on est, je n'ai pas
d'idées pour le faire par texte néanmoins

  Adaptation
	Papier
En papier, il y a tellement de choses à changer. Les guillemets deviennent
lourdes, et l'on aimerait bien transformer un ~6~ en un 6 avec un tilda au
dessus par exemple.

	Signes
J'ai commencé à apprendre la LSF du coup ^^
Je pense qu'avoir un langage uniquement portées sur l'émotions en signes peut
être interessant, mais j'ai encore du mal à voir comment repenser entièrement
repenser la grammaire et les gestes pour en faire quelque chose d'interessant.

  Symboles manquant
Ci contre, la liste des émotions qu'il faudrait peut être ajouter ou
distinguer:
  Admiration
  Ennui?
  Cuteness (A differentier de ç je suppose... Je propose à )
  Stress (A differencier de fatigue?)
  Crush (Trop composite?)
  Dégout (Définitevement je suppose, ça fait partie des cinq émotions universelles)
  Injustice (J'ai l'impression qu'il y a un sentiment de dégout, de frustration et de fatigue. Sans doute trop composite)
