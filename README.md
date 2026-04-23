# Prjet INFO610 - Planning de Staff pour les évenements étudiants

On désire gérer par des moyens informatiques (python) le planning de staff d’un événement BDE.
Pour un événement, il y a différents staff (ex: bar, sono, entrée …) et un certain nombre de staffeur.
Les staffs doivent tourner à chaque créneaux.

On souhaite également compter les heures de staff de chaques personne pour égaliser.

L’utilisateur choisit le timing de ses créneaux, il doit également pouvoir choisir combien de personne il veut pour chaque staff.

En entrée, le programme demande donc :
- **La plage horaire de l’event** (de 21h à 5h)
- **Le timing de roulement** (changement toutes les 1h / 2h)
- **Le nom et genre de chaque personne qui staff**
- **Leur contraintes** (ex: n’aime pas le vomi, le bar …)
- **Le nombre de personne qu’il doit y avoir pour chaque staff** (on choisira surement des valeurs par défaut pour certain staffs).

En sortie:
- Un excel général avec le planning créneau par créneau de tout le monde
- Un planning excel individuel
- Un planning image individuel (taille fond écran tel)


## 2nd temps: Contraintes suplémentaires
- veut staffer avec quelqu’un
- ne veut pas staffer avec quelqu’un
- dispo uniquement à certains créneaux