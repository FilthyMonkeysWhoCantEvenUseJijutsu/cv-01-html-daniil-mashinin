# Crée ton CV HTML en ligne

**C'est ton tour !** Pour t'entraîner, réalise cet exercice étape par étape.

Une fois que tu as terminé, tu peux comparer, auto-évaluer, ton travail avec la **Check-list**

## Contexte

Tu cherches du travail et tu décides de créer ton CV en ligne.
Pour cela, tu vas devoir créer ta première page HTML.

> Pour t'aider, tu peux t'inspirer de [cet exemple de CV](https://divtec-cejef.github.io/101-SFA-HTML-CV-01/)

## Avant de commencer

Suis les cours Treehouse suivants
1. [Introduction to HTML and CSS (2h)](https://teamtreehouse.com/library/introduction-to-html-and-css)
2. [HTML Basics (2-3h)](https://teamtreehouse.com/library/html-basics-2)

_**Alternative :** Fais les 6 chapitres de la [Partie 1 - Maîtrisez les bases de HTML5 ](https://openclassrooms.com/fr/courses/1603881-creez-votre-site-web-avec-html5-et-css3/8061253-tirez-un-maximum-de-ce-cours) du cours [Créez ton site web avec HTML5 et CSS3](https://openclassrooms.com/fr/courses/1603881-creez-votre-site-web-avec-html5-et-css3)_

## Ta mission
1. Crée une nouvelle **branche** `mon-cv-html` dans ton dépôt.
1. Crée et ajoute un fichier `index.html` au dépôt.
1. Lis et mets en pratique les 5 étapes de l'article [Créer une page web de base avec HTML & CSS](https://fallinov.medium.com/cr%C3%A9er-un-page-web-de-base-avec-html-css-2c702e069a0c)
   1. Ajoute les éléments de base à ton fichier `index.html`
   1. Ajoute le reset CSS _Normalize.css_
   1. Crée un fichier CSS de base `main.css` et ajoute les styles de base
   1. Crée et ajoute une **icône** à ton site
   1. Crée la structure de base de ta page avec un **entête**,
      un **contenu principal** et un **pied de page**.
1. Dans l'entête, ajoute une **photo**.
   * Assure-toi qu'un clic dessus ouvre l'image dans un nouvel onglet.
1. Toujours dans l'entête, crée un **menu de navigation** avec **trois liens** vers les sections de ta page. Pour l'instant, laisse les liens vides : `<a href="#">Mon Expérience</a>`
   * Mon expérience
   * Mes compétences
   * Ma formation
1. Dans le contenu principal, insère ton **nom** et ton **prénom** dans un **titre de niveau 1**.
1. Juste après le titre principal, ajoute **trois sections** avec un **titre de niveau 2**.
   * Mon expérience (n'hésite pas à en inventer 😅)
   * Mes compétences (ce que tu maîtrises en informatique)
   * Ma formation (ton parcours scolaire)
   * _Chaque section doit contenir un paragraphe ou une liste à puces._
1. Ajoute une ancre à tes titres de niveau 2 en leur ajoutant un attribut `id`.
    ```html
    <h2 id="experience">Mon Expérience de fou</h2>
    ```
1. Modifie les liens de ton menu pour qu'ils pointent vers tes `id`
    ```html
    <a href="#experience">Mon Expérience</a>
    ```
1. Dans le pied de page, ajoute le copyright, l'année et ton adresse e-mail.
1. Publie ton CV en ligne sur GitHub Pages.
   * [🎥 Vidéo "Créer et publier une page HTML avec GitHub"](https://www.youtube.com/watch?v=W7Appo5snbQ)

> N'oublie pas de **commit** et **push** régulièrement tes modifications sur GitHub.

## Check-list

✅ Ton CV est bien une page HTML.

✅ Ton nom et prénom sont visibles dans l'onglet de la page.

✅ L'icône de la page s'affiche correctement dans l'onglet.

✅ Le contenu de ta page contient un entête `<header>`, un contenu principal `<main>` et un pied de page `<footer>`.

✅ Dans l'entête, on trouve ta photo

✅ Ta photo est un lien cliquable qui ouvre l'image dans un nouvel onglet.

✅ Le menu de navigation te permet d'atteindre les trois sections de ton CV (expérience, compétences, formation).

✅ Le titre principal est un `<h1>` et contient ton nom et prénom.

✅ Ta page a trois sections avec un titre `<h2>` :
  * Mon expérience
  * Mes compétences
  * Ma formation

✅ Chaque section contient au minimum un paragraphe ou une liste à puce.

✅ Dans le pied de page, on voit '©2023' suivi de ton adresse e-mail.

✅ Ton e-mail est un lien cliquable qui permet d'envoyer un e-mail directement.

✅ Ton CV est publié en ligne sur GitHub Pages.

Quand tu as terminé, crée une **Pull Request** `mon-cv-html` et demande une **review** à ton enseignant.

# Prochaine étape
La suite se passe dans le fichier [etape2.md](etape2.md)
