# AFUP
## Meetup 29/04/2025
### Pour un numérique éco-reponsable
#### Exemples d'actions à mener régulièrement, ou à mettre en place :
- nettoyer les fonctions inutilisées : moins de maintenance, de temps dépensé, de bugs qui doublonnent les tentatives d'utilisation (bah oui, quand ça beugge, on retente ou on essaie autrement :) ). Moins de temps de chargement pour les scripts qui doivent être chargés coté client. Et peut-être moins de mémore coté serveur aussi ?
- faire du lazy loading : cela permettra de ne charger les classes/modules/ect que lorsqu'elles sont utilisées, **appelées**.
- services workers : zut, j'aurai dû poser la question. Il me semble que c'est pour pré-charger les fichiers, mais aje ne vois pas ce que ça apporte avec le cache du navigateur, à moins qu'on ne soit capable de mettre à jour le cache sans envoyer tout le fichier, ou bien justement de permettre au navigateur d'avoir une politique de cache "agressive" puisque nous nous forcerons la mise à jour, je ne sais pas.
- Minification : raison évidente : moins de flux de données.
- n'embarquer que le strict nécessaire !!! Pas tout JQuery (par exemple :D )

#### Points d'attention
- Attention aux ORMs : ne pas toujours leur faire confiance. Refaire les jointures manuellement.<br/>
_Note de moi-même : A creuser, car bonne pratique SQL mais semble incompatible avec les bonnnes pratiques de POO... du moins sans connaissances des design patterns adequats_<br/>
- Monitoring : pour bug ou optis, ce qui va permettre, si action s'en suit, de moins consommer de bande passante, de ressources ... <br/>
_Note de moi-même : évidemment, si monitoring sans actions suite à une trouvaille, cela devient finalement une consommation inutile de ressources... A équilibrer entre le fait que cela devienne un support pour peser dans la balance pour faire ou non des optis._
- Attention aux tests qui scannent l'ensemble du code pour le commit d'un fichier...

#### Présentation de l'outil Fruggr
Installé en plusieurs endroits : serveur et extension navigateur<br/>
Cet outil est :
- un outil de mesure de la mise en place des bonnes pratiques de décarbonation
- un outil d'analyse des usages et d'évaluation de l'impact de l'infrastructure (à creuser ^^')

### Symfony UX
- contient pas mal de ficheir JS... même si c'est Symfony !!
- Stimulus : binder JS <-> DOM
#### Avantages 
- Parfois pas besoin de faire du JS du tout
- pas besoin de dupliquer les règles métier dans les vues _Note de moi-même : avec la séparation des couches, à creuser..._
- Front testé en partie, comme le reste du code PHP en tout cas. (pas de end-to-end non plus !!!)
