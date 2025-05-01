# AFUP
## Meetup 29/04/2025
### Pour un numérique éco-reponsable
#### Exemples d'actions à mener régulièrement, ou à mettre en place :
- nettoyer les fonctions inutilisées : moins de maintenance, de temps dépensé, de bugs qui doublonne les tentatives d'utilisation (bah oui, quand ça beugge, on retente ou on essaie autrement :) ). Moins de temps de chargement pour les scripts qui doivent être chargés coté client. Et peut-être moins de mémore coté serveur aussi ?
- faire du lazy loading : cela permettra de ne charger les classes/modules/ect que lorsqu'elles sont utilisées, **appelées**.
- services workers : zut, j'aurai dû poser la question. Il me semble que c'est pour pré-charger les fichiers, mais aje ne vois pas ce que ça apporte avec le cache du navigateur, à moins qu'on ne soit capable de mettre à jour le cache sans envoyer tout le fichier, ou bien justement de permettre au navigateur d'avoir une politique de cache "agressive" puisque nous nous forcerons la mise à jour, je ne sais pas.
- Minification : raison évidente : moins de flux de données.
- n'embarquer que le strict nécessaire !!! Pas tout JQuery (par exemple :D )

#### Points d'attention
Attention aux ORMs : ne pas toujours leur faire confiance. Refaire les jointures manuellement.<br/>
_A creuser, car bonne pratiques SQL mais semble incompatible avec les bonnnes pratiques de POO... du moins sans connaissances des design patterns adequats_<br/>


#### Présentation de l'outil Fruggr
Installé en plusieurs endroits : serveur et extension navigateur<br/>
Cet outil est :
- un outil de mesure de la mise en place des bonnes pratiques de décarbonation
- un outil d'analyse des usages et d'évaluation de l'impact de l'infrastructure (à creuser ^^')
