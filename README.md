# Projet INFO610 - Planning de Staff pour les évenements étudiants
_BRUHAT Thomas - DUPRE Valentin - Groupe A2_

On désire gérer par des moyens informatiques (python) le planning de staff d’un événement BDE.
Pour un événement, il y a différents staff (ex: bar, sono, entrée …) et un certain nombre de staffeur.
Les staffs doivent tourner à chaque créneaux.

On souhaite également compter les heures de staff de chaques personne pour égaliser.

L’utilisateur choisit le timing de ses créneaux, il doit également pouvoir choisir combien de personne il veut pour chaque staff.

En entrée, le programme demande donc :
- **La plage horaire de l’event** (de 21h à 5h)
- **Le timing de roulement** (changement toutes les 1h / 2h)
- **Le nom et genre de chaque personne qui staff**
- **Leur contraintes** (détaillé plus bas)
- **Le nombre de personne qu’il doit y avoir pour chaque staff** (on choisira surement des valeurs par défaut pour certain staffs).
- [ ]
- [x]
En sortie:
- **Un excel général** avec le planning créneau par créneau de tout le monde.
- **Un planning excel individuel**.
- **Un planning image individuel** afin de pouvoir rajouter son planning à son fond d'écran.


## Contraintes et conditions

L'un des problèmes principaux lors de la conception d'un planning est les contraintes individuelles. Chaque personne va avoir des empêchements ou des conditions sur ses capacités ou son intérêt dans un domaine plutôt qu'un autre. Voici donc une liste des principales conditions qui sont récurentes et que nous prendrons en compte dans notre code (attributs, conditions SQL...)

- **Est déjà pris dans un créneau** : Cela peut paraitre sensé mais il faut poser dans le code les bases et le fondement du planning.

- **Le genre et les toilettes** : Nous devons préciser dans la classe Staff le genre (H/F) de la personne afin de l'attribuer aux toilettes Homme ou Femme correspondante.

- **Les affinités** : Pour simplifier les roulements et rendre la soirée agréable pour le staff, les créneaux se feront en binome qui s'entendent bien (avec qui ils "aimeraient travailler"). Traditionnellement, un sondage au sein du BDE est fait pour connaitre les envies de chacun et avec qui veulent-ils être en binome.

- **Les responsables de pôles** : Les responsables de pôles doivent être présent au poste où ils sont responsable durant la totalité ou la majorité de la soirée.

- **L'équilibre des heures de staff** : Une harmonie des heures de staff doit être respecté. Une personne A staffant 12 heures alors qu'une personne B staffant 2h n'est pas viable. Il faut donc ajouter une condition d'harmonisation des heures afin de répartir au mieux les charges de staff.