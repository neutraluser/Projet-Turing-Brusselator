
# Motifs de Turing dans un système de réaction-diffusion : modèle de Brusselator

## Introduction

Les systèmes de réaction-diffusion sont des modèles mathématiques permettant de décrire l'évolution spatiale et temporelle de plusieurs espèces chimiques. Ils reposent sur deux phénomènes complémentaires : les réactions chimiques locales, qui transforment les espèces les unes en les autres, et la diffusion, qui permet leur propagation dans l'espace.

En 1952, Alan Turing a montré que la diffusion pouvait déstabiliser un état homogène et conduire à l'apparition de structures spatiales organisées, appelées **motifs de Turing**. Ces motifs peuvent prendre différentes formes, notamment des taches ou des bandes. Ils sont observés dans de nombreux phénomènes naturels, comme les motifs présents sur la peau des zèbres, des léopards ou de certains poissons.

Ce projet a pour objectif d'étudier la formation de ces motifs à travers le modèle de réaction-diffusion du **Brusselator**, proposé par Ilya Prigogine et ses collaborateurs.

## Objectifs du projet

Le travail est organisé autour de plusieurs étapes :

1. **Analyse de stabilité linéaire :** déterminer les conditions d'apparition de l'instabilité de Turing et calculer le seuil critique.
2. **Simulation en une dimension (1D) :** discrétiser les équations, implémenter un schéma numérique et étudier la stabilité des simulations.
3. **Simulation en deux dimensions (2D) :** reproduire numériquement les motifs de Turing et observer leur évolution.
4. **Caractérisation des motifs :** analyser les structures obtenues, mesurer leurs longueurs d'onde et identifier les motifs en bandes ou en hexagones.
5. **Extensions :** étudier éventuellement l'hystérésis ou l'application du modèle à l'électrodéposition dans les batteries.

## Modèle étudié

Le modèle du Brusselator est décrit par le système d'équations aux dérivées partielles suivant :

$$
\frac{\partial X}{\partial t}
= A-(B+1)X+X^2Y+\nabla^2X
$$

$$
\frac{\partial Y}{\partial t}
= BX-X^2Y+D\nabla^2Y
$$

où :

- $X$ représente l'activateur ;
- $Y$ représente l'inhibiteur ;
- $A$ est un paramètre fixé ;
- $B$ est le paramètre de contrôle ;
- $D$ est le rapport des coefficients de diffusion.

## Outils utilisés

- Python
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook
- Git et GitHub

## Paramètres de référence

Les simulations utiliseront principalement les paramètres suivants :

- $A = 4.5$
- $D = 8$

L'objectif final est de reproduire les motifs de Turing obtenus par simulation numérique et d'étudier leur apparition en fonction des paramètres du modèle.

## Références bibliographiques

- A. M. Turing (1952), *The Chemical Basis of Morphogenesis*.
- B. Peña et C. Pérez-Garcia (2001), *Stability of Turing Patterns in the Brusselator Model*.
