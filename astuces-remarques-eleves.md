# Astuces et remarques pour une meilleure revue de code HTML et CSS

Voici un guide organisé pour regrouper les remarques et astuces élaborées lors des revues de code. Ce document est divisé en deux parties : **HTML** et **CSS**.

---

## **HTML**

### Organisation et Structure

- Organisez votre site avec des dossiers structurés :

  ```
  racine-de-mon-site
    ├── css
    │   └─ main.css
    │   └─ fonts.css
    ├── fonts
    │   └─ arial.woff
    │   └─ arial.ttf
    ├── img
    │   └─ logo.svg
    │   └─ photo-plage.jpg
    ├─ favicon.ico
    └─ index.html
  ```

- Utilisez des noms de fichiers et de dossiers **en minuscules**, sans espaces ni caractères spéciaux (exemple : `css/trop-style.css`).

- La page d’accueil doit obligatoirement être nommée **`index.html`**.

### Meilleures Pratiques de Balises

- **Langue** : Définissez la langue dans l'attribut `<html lang="fr">` (ou autre).

- **Titre** : Ajoutez un `<title>` pertinent, correspondant au titre principal de votre site.

  ```html
  <title>Tout l’assortiment de jouets | Migros</title>
  ```

- **Meta Viewport** : Assurez-vous que votre site est adapté aux smartphones.

  ```html
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  ```

- **Favicon** : Incluez une icône de site.

  ```html
  <link rel="icon" href="favicon.ico">
  ```

### Règles de Code

- **Indentation** : Indentez avec 2 ou 4 espaces.

  ```html
  <main>
    <h1>Mon titre</h1>
    <p>Mon paragraphe</p>
  </main>
  ```

- **Pas d’espaces inutiles** :

  ```html
  <!-- Faux -->
  <ul class = "sommaire">
  <!-- Juste -->
  <ul class="sommaire">
  ```

- **Balises `<p>`** : Contiennent des phrases complètes, pas de simples mots.

- **Textes Inline uniquement** : Les `<p>` ne doivent contenir que des balises inline (`<strong>`, `<em>`, `<a>`, etc.).

- **Texte alternatif** : Utilisez `alt` pour décrire vos images.

  ```html
  <img src="img/fifty-burgers.png" alt="Logo Fifty Burgers">
  ```

- **Séparation logique** : Séparez votre contenu en `<header>`, `<main>` et `<footer>`.

- **Pas de `<br>` pour les espacements** : Utilisez les styles CSS (padding/margin).

- **Structure sémantique** : Privilégiez les balises sémantiques appropriées (`<article>`, `<section>`, `<aside>`, etc.) pour organiser votre contenu.

### Validation et Accessibilité

- **Entités HTML** : Préférez `&copy;` pour `©`.
- **Pas de tailles d’images en HTML** : Préférez CSS.
- **Fin de fichier** : Ajoutez une ligne vide en fin de fichier.
- **Validation** : Utilisez [W3C Validator](https://validator.w3.org/nu/).

---

## **CSS**

### Organisation et Structure

- **Nom des classes** : Privilégiez des noms clairs et représentatifs.

- **Espaces** : Toujours un espace avant les accolades et entre les blocs.

  ```css
  h1 {
      color: red;
  }
  
  p {
      color: blue;
  }
  ```

- **Revenir à la ligne** : Après une `,` dans les sélecteurs multiples.

  ```css
  h1,
  h2,
  h3 {
      color: red;
  }
  ```

### Bonnes Pratiques de Style

- **Liens** : Définissez leur style et leur hover.

  ```css
  a {
      color: red;
  }
  a:hover {
      color: blue;
  }
  ```

- **Fluidité des images** :

  ```css
  img {
      max-width: 100%;
      height: auto;
  }
  ```

- **Unités** : Préférez `rem` ou `em` à `px`.

- **Couleurs** : Toujours écrire les noms de couleurs en minuscules.

- **Fontes** : Toujours définir une famille de secours (exemple : `sans-serif`).

  ```css
  body {
      font-family: "Roboto", sans-serif;
      font-size: 1.2rem;
      font-weight: normal;
      line-height: 1.4;
  }
  ```

### Optimisation

- **Unité inutile pour `0`** :

  ```css
  margin: 0; /* et non 0px */
  ```

- **Images d’arrière-plan** : Mettez les URL entre guillemets.

  ```css
  background-image: url("https://example.com/image.jpg");
  ```

- **Outils d’optimisation** : Minifiez vos fichiers CSS avant leur mise en production pour réduire leur poids. Utilisez des outils comme PostCSS ou Autoprefixer pour ajouter automatiquement les préfixes nécessaires.

---

Adoptez ces bonnes pratiques pour améliorer la qualité de votre code et en faciliter la maintenance. Bonne continuation dans vos projets web !
