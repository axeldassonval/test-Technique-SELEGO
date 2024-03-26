# test-Technique-SELEGO

J'ai effectué les corrections des bugs suivants :

Vue utilisateur :

- Le champ "name" était désactivé, j'ai retiré l'attribut "disabled" afin de permettre la modification du nom.
- J'ai observé une erreur de fonctionnement sur le bouton "update", j'ai corrigé en remplaçant "onChange" par "onClick".

Projet :
- Une erreur de rendu de la page due à l'utilisation de la fonction "toString" dans la partie HTML de l'application. Je l'ai remplacée par "String(project.name)" qui fonctionnait dans ce cas d'utilisation.
- Erreur dans la fonction "setProject" qui attribuait un tableau à la variable "project", rendant toutes les valeurs du rendu "undefined". Corrigé en remplaçant "setProject(u)" par "setProject(u[0])".

Édition de projet :
- Erreur dans la fonction "setProject" qui attribuait un tableau à la variable "project", empêchant ainsi le pré-remplissage du projet. Corrigé en remplaçant "setProject(u)" par "setProject(u[0])".
- Le champ "name" était désactivé, j'ai retiré l'attribut "disabled" pour permettre la modification du nom du projet.

Nouvelle fonctionnalité :
J'ai décidé d'ajouter un composant "CancelButton". Comme son nom l'indique, il a pour objectif d'annuler les actions en cours et de rediriger vers la page précédente. Je pense qu'il est pertinent de l'ajouter pour un meilleur confort utilisateur lors de la manipulation des formulaires, afin d'éviter la suppression involontaire d'un projet.

Retour d'expérience :
Lors de mes recherches, j'ai observé plusieurs erreurs liées à l'attribution des clés dans les listes, des valeurs attribuées à "null" et la recommandation d'utiliser des chaînes vides ou encore "Input elements should not switch from uncontrolled to controlled". J'ai également remarqué de nombreux "console.log". Oubliés ou laissés volontairement dans le code, il pourrait être intéressant d'ajouter un logger pour ces cas, ce qui serait plus propre. Je n'ai pas rencontré de difficultés majeures lors de mes recherches.

