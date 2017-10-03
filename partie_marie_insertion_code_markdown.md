## Afficher du code

### Pour afficher du code avec coloration syntaxique en Markdown

Il est possible d'afficher une portion de code tout en maintenant sa coloration syntaxique grâce au markdow.

Pour un bloc de code, procéder en indentant tout simplement le code (touche tab ou 4 espaces)


**Exemple**:
Voici un code en C :

    <script type="text/javascript">
      alert("Hello!");
    </script>

### Pour afficher du code de type instructions dans une ligne de texte en Markdown

Si on veut non pas ajouter tout un bloc de code mais uniquement montrer visuellement qu'une partie du texte dans une phrase est une instruction en code, on entoure celle-ci avec un caractère spécial ressemblant à un apostrophe inversée.

Pour trouver ce caractère sur votre clavier, il faut utiliser la combinaison de touches Alt Gr + 7 ou la combinaison Alt GR + £ . Attention taper deux fois de suite l'un de ces raccourcis clavier pour voir apparaitre le caractère.

**Exemple**:

La fonction `printf()` permet d'afficher du texte


## Séparer deux blocs de code

Il peut être génant lorsque l'on veut placer deux blocs de code l'un à la suite de l'autre qu'il s'affiche dans un seul et même bloc. Pour éviter cela, il faut séparer les deux blocs avec un ligne de commentaire html qui n'apparaitra pas à l'écran.

Les commentaires en html s'écrive comme ceci : `<!-- texte en commentaire -->;`

**Exemple**:

  <script type="text/javascript">
      alert("Hello!");
  </script>

<!-- Commentaire html -->

  <script type="text/javascript" >
      window.alert("Hello World!");

      alert("Hello World!");
  </script>
