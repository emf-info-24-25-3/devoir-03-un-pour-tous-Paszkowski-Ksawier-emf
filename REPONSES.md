## REPONSES :
1. Peut-on modifier l'âge d'un chien une fois qu'il a été créé (essayez de donner 10 ans à chien3 pour vérifier) ? 

Non, car l'attribut age est privé et il n'y a pas de méthode pour le modifier.

2. Que se passe-t-il si on modifie le nom de chien2 ?

Tous les chiens prendront ce nouveau nom, car nom est static et partagé par toutes les instances.

3. Pourquoi tous les chiens ont tous le même nom ?

Parce que nom est static, donc il est commun à tous les objets Chien.

4. Observez avec attention les lignes N°20 à N°26 du main() et réfléchissez : par quel miracle le chien3 à la ligne N°26 s'affiche correctement ?
   Répondez à cette question en expliquant avec précision ce qui se passe et pourquoi.

```java
System.out.println(chien3);
```
appelle toString(), qui affiche nom et age.
Mais à cause de static, le nom affiché sera le dernier assigné.

