# MyInk

MyInk est une application de bureau pour créer et lire des livres interactifs. L'histoire est composée de pages reliées par des choix ; certains chemins peuvent nécessiter des objets obtenus pendant la lecture.

L'éditeur permet d'organiser les pages sous forme de graphe, de modifier leur contenu et d'ajouter des objets. Les livres valides peuvent être lus dans l'application et exportés en PDF. La bibliothèque permet aussi de dupliquer ou supprimer un livre.

## Technologies

- Java 21 et JavaFX 21, avec FXML et CSS pour l'interface.
- Maven pour la compilation et la gestion des dépendances.
- RichTextFX pour le texte enrichi et Apache PDFBox pour l'export PDF.
- JUnit 5 pour les tests.

## Lancer le projet

Installez un JDK 21 et placez-vous à la racine du projet. Le Maven Wrapper télécharge Maven et les dépendances si nécessaire.

Sur macOS ou Linux :

```sh
./mvnw clean javafx:run
```

Sur Windows :

```bat
mvnw.cmd clean javafx:run
```

## Sauvegarde des livres

Les livres sont enregistrés dans un dossier `MyInkBooks` situé dans le répertoire de lancement de l'application.

## Distributions autonomes

Le workflow GitHub Actions **Distributions autonomes**, lancé manuellement depuis l'onglet Actions, construit des paquets pour macOS ARM64, Windows x64 et Linux x64. Une fois la construction terminée, téléchargez les trois archives dans la section **Artifacts** de l'exécution. Les paquets incluent Java et ne nécessitent donc pas son installation séparée.

Les paquets ne sont pas signés. Leur installation et leur fonctionnement doivent être vérifiés sur chaque système cible.

## Crédits

- Asmaou B.
- Melissa Y.
- Yanis N.
