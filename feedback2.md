
Etape 1 
  La route est ok, le controller manque de sécurité, priviléige plutôt une requête prepraé avec $1 comme vu en cours, ça evitera les injections SQL
  Pour les prochaines fois pense NTUI (Never Trust User Input)
  tu aurais pu faire un Number(id) ou un ParseInt(id) pour éviter cela
  Dasn ton DataMapper, pourquoi appeler 2 fois le même fichier? 

Etape 2
  Très bien de vouloir faire la recherche des cartes sans element, mais ce n'est pas ce qui a été demandé.
  Le plus simple aurait été de faire 2 requetes bien différentes avec un if else
  Pour l'affichage, tu avais déjà une page toute faite, il aurait fallu faire une render sur la page CardList avec pour exemple le mainController

Etape 3

  3.1 
  Ne cherche pas à changer les paramètres que tu as pu voir en cours, si tu as un doute reprends juste la documentation. Pour le coup la sécurité de ta session peut être corrompte avec cookie secure false

  3.2 
  Même commentaire pour le rendu de la page que précédemment, un render avec CardList aurait suffit
  Ne te complique pas la vie, un dev fait au plus simple, il va utilisé la méthode DRY (Don't Repeat Yourself)
  Dans ton controller, tu n'as pas mis en place le nombre maximum de carte dans le deck, tu as le droit de faire un if dans un if

  3.3 
  Petit coquille dans ton render de deck ($)
  Même commentaire pour le render



N'oublie pas qu'il n'y pas d'obligation de finir impérativbement un parcours, le but est que tu puisses mettre en application avec ce que tu as compris les cours de cette saison
Arrête toi sur une étape entièrement fini plutôt que de partir dans tous les sens
La tortue arrive en premier contre le lièvre :p

J'espère que tu as pu faire la correction avec tes camarades de formation et que tu as pu poser les questions nécessaire pour mieux comprendre l'ensemble
Si tu as besoin d'explications sur le code de la correction reviens me voir
Essaie de faire attention à tes sécurités en règle général
Ne t'inquiètes pas trop, tu vas pouvoir t'excercer sur les prochains challenges