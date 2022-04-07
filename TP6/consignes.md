Exercice 1 :
En Italie, chaque personne possède un code d'identification unique délivré par l'administration fiscale nationale après l'enregistrement de la
naissance : le code fiscal (Codice Fiscale). Consultez la page https://en.wikipedia.org/wiki/Italian_fiscal_code pour plus d’informations
Vous aurez à disposition un objet contenant les données personnelles d'une personne (nom, prénom, sexe et date de naissance), Créer une
fonction fiscalCode qui renvoie les 11 caractères du code sous forme de chaîne de caractères en suivant ces étapes :
Générez 3 lettres majuscules à partir du nom de famille, s’il y a:
Au moins 3 consonnes,prendre les 3 premières consonnes. (Newman -> NWM).
Moins de 3 consonnes, les voyelles remplaceront les caractères manquants dans le même ordre qu'ils apparaissent (Fox -> FXO | Hope ->
HPO). Moins de trois lettres, "X" prendra le troisième emplacement après la consonne et la voyelle (Yu -> YUX).
Générez 3 lettres majuscules à partir du nom, s’il y a :
Exactement 3 consonnes ,les consonnes sont utilisées dans l'ordre où elles apparaissent (Matt -> MTT). Plus de 3 consonnes , la première,
troisième et quatrième consonnes sont utilisées (Samantha -> SNT | Thomas -> TMS).
Moins de 3 consonnes, les voyelles remplaceront les caractères manquants dans le même ordre qu'ils apparaissent (Bob -> BBO | Paula ->
PLA).
Moins de trois lettres, "X" prendra le troisième emplacement après la consonne et la voyelle (Al -> LAX).
Générez 2 chiffres, 1 lettre et 2 nombres à partir de la date de naissance et du sexe :
Prenez les deux derniers chiffres de l'année de naissance (1985 -> 85).
Générez une lettre correspondant au mois de naissance (janvier -> A | décembre -> T) en utilisant la table de conversion incluse dans le code.
Pour les hommes, prenez le jour de naissance en ajoutant un zéro au début s'il est inférieur à 10 (tout 9e jour -> 09 | tout 20e jour -> 20).
Pour les femmes, prenez le jour de naissance et ajoutez 40 (tout 9e jour -> 49 | tout 20e jour -> 60).
Les lettres de code doivent être en majuscules.
La date de naissance est indiquée dans le format J/M/AAAA.
Y n'est pas une voyelle.
La table de conversion des mois est la suivante :
Janvier = A
Février = B
Mars = C
Avril = D
Mai = E
Juin = H
Juillet = L
Août = M
Septembre = P
Octobre = R
Novembre = S
Décembre = T


2. Écrire une fonction prop_access(object, path) qui prend en paramètre un chemin et un objet et retourne la valeur associée.
Si l’attribut n'existe pas alors retourné le chemin + “not exist” ( ex: “post.comments.type not exist”
Si le chemin est vide Renvoyez l’objet complet.
