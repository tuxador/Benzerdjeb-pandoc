# Comment rédiger un rapport avec markdown/pandoc

## Intro:
voici mon workflow "idéal" pour rédiger *vite et bien* nos rapports médicaux et opératoires.

## pré-requis:
- Avoir sur sa machine les logiciels **pandoc** et la suite **latex** (tex-live avec les paquets qu'il faut)
- Se placer dans le répértoire de travail que j'ai nommé Benzerdjeb-pandoc.
- Connaitre le minimum de la syntaxe **markdown** (le minimum s'apprend en 10 minutes, le maximum en moins d'une heure ;))
- Ne pas avoir peur de la ligne de commande.

## Comment faire:   

- Rédiger le rapport en markdown (modèle déjà disponible) et le sauvegarder ex: monPatient.md
- ouvrir le terminal dans ce répértoire de travail (en appuyant sur F4 par ex) et lancer la commande:

> Pandoc -S -s --latex-engine=xelatex --template=template-medical.tex MonPatient.md -o MonPatient.pdf

Pour les rapports de coro on utilise '--template=template-coro.tex' à la place du template-medical.

## Crédit:

travail humblement réalisé par le Dr.Yahyaoui en utilisant des logiciels entièrement libres et gratuits.

À partager bien sûr et à *customiser* selon les besoins.