# Exercice : somme d'un fichier de nombres

## Énoncé

Écrire un programme qui lit un fichier texte contenant **un nombre entier par
ligne** et qui affiche **la somme de ces nombres** dans la console.

Exemple — fichier fourni `numbers.txt` :

```
10
20
30
40
50
```

Résultat attendu :

```
Somme = 150
```

## Démarrage

```bash
mvn spring-boot:run -Dspring-boot.run.arguments=numbers.txt
```

Ou avec le jar packagé :

```bash
mvn package
java -jar target/sum-upload-0.0.1-SNAPSHOT.jar numbers.txt
```

## À faire

Le code à implémenter se trouve dans
`src/main/java/fr/interview/sum/SumRunner.java` (méthode `sum`, marquée `TODO`).

- Le fichier est lu ligne par ligne dans `run()` — il ne reste qu'à parser
  chaque ligne et additionner.
- Pas besoin de gérer les erreurs (ligne vide, fichier mal formé, etc.) —
  le cas nominal suffit.
- Durée indicative : 10 minutes.
