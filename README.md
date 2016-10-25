# thesis-tex

<i> Mots clés : Édition collaborative, décentralisé, temps réel, Web, passage à
l'échelle, structure de données répartie pour séquences, échantillonnage
aléatoire de pairs.  </i>

<i> Keywords: Collaborative editing, decentralized, real-time, Web, scalable,
replicated structure for sequences, random peer sampling.  </i>

LaTeX sources of my [Ph.D
manuscript](https://github.com/Chat-Wane/thesis-tex/blob/master/manuscript.pdf) about
decentralized collaborative editing on the Web (written in French).

## Résumé

Un éditeur collaboratif permet de répartir la tâche de rédaction d'un document à
travers le temps et l'espace. Par leur simplicité d'utilisation, les éditeurs
collaboratifs temps réel du Web ont contribué à l'adoption massive de ces outils
par le grand public. Cependant, les éditeurs actuels sont centralisés : un
serveur appartenant à un fournisseur de services gère une session d'édition. En
résultent des problèmes de confidentialité, de censure, de propriété, de passage
à l'échelle et de tolérance aux pannes.

Récemment, la possibilité d'établir des communications d'un navigateur Web à
l'autre a ouvert de nouvelles opportunités en faveur d'un Web décentralisé. Un
éditeur collaboratif temps réel décentralisé fonctionnant dans les navigateurs
Web doit gérer efficacement des groupes de taille variable et hautement
dynamiques.

Cette thèse comporte trois contributions :
<ol type="i">
  <li> Pour représenter le document, nous proposons une structure de données
    répliquée dont la taille des métadonnées croît de manière sous-linéaire par
    rapport au nombre de caractères insérés dans le document. </li>
  <li> Pour propager efficacement les changements à tous les éditeurs
    participant à l'édition, nous proposons un protocole d'échantillonnage
    aléatoire de pairs adapté aux contraintes des navigateurs Web et s'ajustant
    automatiquement au logarithme de la taille de la session d'édition. </li>
  <li> Pour démontrer la faisabilité d'un éditeur collaboratif temps réel
    décentralisé fonctionnant dans les navigateurs Web, nous proposons un
    éditeur réunissant (i) et (ii), et dont les performances passent à
    l'échelle. </li>
</ol>

## Abstract

Collaborative editors allow users to distribute the writing of a document across
space and time. Thanks to their ease of use, real-time collaborative editors
working in Web browsers vastly contributed to the adoption of such
tools. However, current editors are centralized: a service provider's server
hosts an editing session. It raises privacy and scalability issues.
  
Recently, the enabling of browser-to-browser connection establishments opened
new opportunities in favor of a decentralized Web.  Decentralized real-time
collaborative editors working in Web browsers must efficiently handle highly
dynamic groups of different size.

Contributions of this thesis are threefold:
<ol type="i">
  <li> To represent the document, we propose a replicated data structure for
    sequences using metadata the size of which scales sub-linearly compared to
    the number of inserted characters. </li>
  <li> To efficiently propagate the changes to all editors involved in the
    collaborative writing, we propose a random peer sampling protocol that
    supports Web browsers constraints and self-adjusts its functioning to the
    variations of network membership.</li>
  <li> To demonstrate the feasibility of a decentralized real-time
    collaborative editors running in Web browsers, we propose an editor using
    (i) and (ii), and we highlight its scalability. </li>
</ol>


## Compile

It requires the font [Crimson](http://www.fontsquirrel.com/fonts/crimson).

```
$ xelatex paper.tex
$ bibtex paper
$ xelatex paper.tex
```

## Acknowledgments

This work was partially funded by the French ANR project
[ConcoRDanT](http://concordant.lip6.fr) (ANR-10-BLAN-0208), the French ANR
project [SocioPlug](http://socioplug.univ-nantes.fr/) (ANR-13-INFR-0003), and by
the [DeSceNt](http://www.descent.cominlabs.ueb.eu/) project granted by the Labex
CominLabs excellence laboratory (ANR-10-LABX-07-01).

