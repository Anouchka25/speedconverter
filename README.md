Classe SpeedConverter
1. Écrivez une méthode appelée toMilesPerHour qui a 1 paramètre de type double avec le nom kilometersPerHour. Cette méthode doit renvoyer la valeur arrondie du calcul de type long.

Si le paramètre kilometersPerHour est inférieur à 0, la méthode toMilesPerHour doit renvoyer -1 pour indiquer une valeur non valide.


Sinon, si elle est positive, calculez la valeur des miles par heure, arrondissez-la et renvoyez-la. Pour la conversion et l'arrondi, consultez les notes dans le texte ci-dessous.

Exemples d'entrée / sortie:
* toMilesPerHour(1.5); → devrait retourner une valeur 1
* toMilesPerHour(10.25); → devrait retourner une valeur 6
* toMilesPerHour(-5.6); → devrait retourner une valeur -1
* toMilesPerHour(25.42); → devrait retourner une valeur 16
* toMilesPerHour(75.114); → devrait retourner une valeur 47


2. Ecrire une autre méthode printConversion avec 1 paramètre de type double avec le nom kilometersPerHour.

Cette méthode ne doit rien renvoyer (void) et elle doit calculer milesPerHour à partir du paramètre kilometersPerHour.

Il doit ensuite imprimer un message au format "XX km / h = YY mi / h".

XX représente la valeur d'origine kilometersParHeure.
YY représente les miles arrondis par heure à partir du paramètre kilomètres par heure.

Si le paramètre kilometresHeure est <0, imprimez le texte "Valeur invalide".


Exemples d'entrée / sortie:
* printConversion(1.5); → devrait imprimer le texte suivant (dans la console - System.out): 1.5 km/h = 1 mi/h
* printConversion(10.25); → devrait imprimer le texte suivant (dans la console - System.out): 10.25 km/h = 6 mi/h
* printConversion(-5.6); → devrait imprimer le texte suivant (dans la console - System.out): Invalid Value
* printConversion(25.42); → devrait imprimer le texte suivant (dans la console - System.out): 25.42 km/h = 16 mi/h
* printConversion(75.114); → devrait imprimer le texte suivant (dans la console - System.out): 75.114 km/h = 47 mi/h


Use method Math.round to round the number of calculated miles per hour(double). The method round returns long.
Utilisez la méthode Math.round pour arrondir le nombre de miles calculés par heure (double). La méthode arrondir retourne un long.


Comment utiliser la méthode round et comment ça marche?

Math.round () est une méthode mathématique intégrée qui renvoie la longueur la plus proche de l'argument. Le résultat est arrondi à un entier en ajoutant 1/2, en prenant la part du résultat après avoir ajouté 1/2 et en transtypant le résultat en type long. La méthode renvoie la valeur de l'argument arrondie à la valeur int la plus proche.


EXEMPLE D'UTILISATION:

double number = 1.5;
long rounded = Math.round(number);
System.out.println("rounded= " + rounded);
System.out.println("with 3.9= " + Math.round(3.9));
System.out.println("with 4.5= " + Math.round(4.5));
int sum = 45;
int count = 10;
// transtypage de sorte que le résultat est double, par exemple / int -> double
double average = (double) sum / count;
long roundedAverage = Math.round(average);
System.out.println("average= " + average);
System.out.println("roundedAverage= " + roundedAverage);


OUTPUT:

rounded= 2
with 3.9= 4
with 4.5= 5
average= 4.5
rounded Average= 5


CONSEIL: Dans la méthode printConversion, appelez la méthode toMilesPerHour au lieu de dupliquer le code.

REMARQUE: toutes les méthodes doivent être définies comme statiques publiques.
REMARQUE: 1 mile par heure est 1,609 kilomètres par heure
REMARQUE: n'ajoutez pas de méthode principale au code de la solution.
