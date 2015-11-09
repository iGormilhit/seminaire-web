# Séminaire web

Participation à un cours de la [HEG](http://www.hesge.ch/heg), dans la filière *Information documentaire*.

Il s'agit de présenter un article scientifique en rapport avec le *Web*. Pour ma part, j'ai choisi l'article suivant :

DOTY, Nick, 2015. Reviewing for Privacy in Internet and Web
Standard-Setting. In : *2015 IEEE Security and Privacy Workshops (SPW)*
\[en ligne\]. mai 2015. pp. 185‑192. Disponible à l’adresse :
http://dx.doi.org/10.1109/SPW.2015.18

[PDF](pdf/reviewing_for_Privacy_in_Internet_and_Web_Standard.pdf)

Le but de ce dépôt est d'y rassembler : 

   * mes [notes de lectures](notes/lecture.md), [structure](notes/structure.md) du texte.
   * le texte de ma présentation (*well, maybe*),
   * les slides.

Le tout, si possible, en *MarkDown*, avec des conversions en PDF, ePub et html via *pandoc*.

## Slides

Pour la partie *slides*, il faut copier le dépôts ``reveal.js`` dans le dossier ``slides``, par exemple :

```bash
$ cd slides
$ git clone https://github.com/hakimel/reveal.js.git
```

Pour générer les slides en ``html`` avec pandoc :

```bash
$ pandoc -s -t revealjs -o slides.html slides.md
```
