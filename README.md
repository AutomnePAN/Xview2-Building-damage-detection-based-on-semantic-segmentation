# Nuit de l'IA - Evaluation de bâtiments endommagés après des catastrophes naturelles

## Dataset : XBD
Le dataset utilisé est le dataset xBD publié en 2019 : voir http://openaccess.thecvf.com/content_CVPRW_2019/papers/cv4gc/Gupta_Creating_xBD_A_Dataset_for_Assessing_Building_Damage_from_Satellite_CVPRW_2019_paper.pdf 
Il consiste en des images satellites de taille 1024x1024 avant et après des catastrophes naturelles, ainsi que des labels indiquant où se situent les bâtiments dans l'image, ainsi que leur état de dommage après la catastrophe.

## Challenge Xview2
Ce dataset est utilisé actuellement dans le challenge xView2 (https://www.xview2.org/), organisé par le Defense Innovation Unit des Etats-Unis. Le but du challenge est de conduire à la création d'algorithmes permettant une meilleure analyse des zones venant de subirune catastrophe naturelle.

<br/>

## Problème du Hackathon
Pour chaque paire d'images avant-après catastrophe, l'objectif est d'évaluer la position des buildings et leur état de destruction.

[IMAGE]

L'état de destruction est défini selon une échelle de 4 niveaux:
 - 1 : pas de dégâts
 - 2 : dégâts mineurs
 - 3 : dégâts majeurs
 - 4 : détruit


## Objectifs
L'évaluation des dégâts des buildings sera une matrice de taille 1024x1024 à valeur dans {0,1,2,3,4}, classifiant chaque pixel comme 0 (pas de building) ou un niveau de dégât entre 1 et 4. Une fonction d'évaluation est prévue (voir le notebook).

Cette mesure est celle du challenge xView2. Vous êtes bien sûr libres de créer d'autres mesures et de reformuler le problème. En ce cas, à vous de convaincre le jury de l'intérêt et de la difficulté de votre formulation.
