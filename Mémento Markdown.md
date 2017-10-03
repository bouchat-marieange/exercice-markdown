

# Exercice-markdown
Exercice markdown et github en collaboration

### Navigation
[README.md](https://github.com/bouchat-marieange/exercice-markdown/blob/master/README.md)

[Présentation Markdown.md](https://github.com/bouchat-marieange/exercice-markdown/blob/master/Pr%C3%A9sentation%20Markdown.md)

[Mémento Markdown.md](https://github.com/bouchat-marieange/exercice-markdown/blob/master/M%C3%A9mento%20Markdown.md)

### Les Titres

Les titres en Markdown sont précédés du signe "#"(dièse)
et le nombre de dièse se situant devant le titre définissent le
niveau du titre. Ainsi un dièse devant du texte, sera l'équivalent d'un titre h1 en html,
deux dièse pour un titre h2 etc...

##### Exemple :  

````
# titre1  
## titre2   
### titre3
````

##### Resultat :
# titre1   
## titre2  
### titre3


### Les Paragraphes

Markdowns permet de mettre en évidence certaines parties du texte dans les paragraphes. Entourer
le texte d'astérisques permet de le rendre italique, l'entourer de double astérisques
le rendent gras. Les triples astériques permettent, d'accentuer la mise en évidence en combinant les
deux effets précédents.

##### Exemple :  

````
*mon texte italique*
**mont texte gras**   
***mon texte italique et gras***
````

##### Resultat :
*texte*   
**texte**     
***texte***

# Les différentes listes
Cette partie traitera de l'ajout de listes à puces, de listes numériques ainsi que de listes imbriquées.

Nous commencerons par expliquer comment les ajouter de manière très simple suivis d'un exemple en image pour chaque listes.

## 1. La liste à puces:

Lorsque vous avez plusieurs élément à afficher dans une liste non-ordonnée (sans numérotation),
il vous suffi de commencer chaque ligne de code par une * suivis d'un espace puis de l'élément à lister.

Par exemple:
* Belgique
* Allemagne
* France
* . . .

Comment y arriver ?
````
* Belgique
* Allemagne
* France
* . . .
````

## 2. La liste numérique:

Imaginons que, suite à une compétition, vous avez un classement à afficher. C'est dans cette rubrique que vous trouverez la manière d'y parvenir.  
Il vous suffira de commencer la liste par un 1. suivis d'un espace puis de l'élément à placer en 1er.   
Ce qui diffère de la liste à puces, c'est qu'il faudra commencer les lignes suivantes par 2. , 3. , etc..

Par exemle:
1. Belgique
2. Allemagne
3. France

Voici comment faire:   
````
1. Belgique
2. Allemagne
3. France
````

## 3. La liste imbriquées:

Il est aussi possible d'imbriquer une liste dans une autre lorsque vous avez besoin d'afficher des sous-éléments.

###### Liste à puces:
* Belgique
  * Bruxelles
* Allemagne
  * Berlin
* France
  * Paris

###### Liste numérique:
1. Belgique
    1. Bruxelles
    2. Anvers
2. Allemagne
    1. Berlin
3. France
    1. Paris

Pour avoir le même résultat, il faudra simplement créer un tabulation (appuyez sur la touche Tab de votre claier) puis procéder de la même façon que sur les exemples précédents.
````
* Belgique
  * Bruxelles
* Allemagne
  * Berlin
* France
  * Paris
````
PS: pour la liste numérique imbriquée, il vous faudra commencer par 4 espaces avant d'énumérer vos éléments.

# Comment insérer un lien ou une image en MarkDown ?

## Liens

Contrairement au Html où l'utilisation de balises était nécessaire, en MarkDown, il suffit de *placer le texte du lien entre crochets suivis de l'URL entre parenthèses*. Voyons comment cela fonctionne en pratique, avec la page d'OpenClassRooms qui est notre principale source d'inspiration. Je tape le texte "OpenClassRooms" entre [] et j'insère le lien entre parenthèses juste après : `[texte](Lien)`. Exemple : [OpenClassRooms](https://openclassrooms.com/courses/redigez-en-markdown).

## Images

Pour ce qui est des images, le principe est le même, à la seule différence qu'il faut rajouter un point d'exclamations juste avant les crochets : `![texte alternatif](lien de l'image)`. Pour l'exemple, après de longues discussions, il a été décidé d'utiliser le Pingouin Ninja : ![Pingouin Ninja](https://www.spreadshirt.be/image-server/v1/mp/designs/14527900,width=178,height=178/pingouin-ninja.png)

## Images animées

Afin de vous exprimer notre gratitude, notre dino-dabeur tenait à vous faire une démonstration des images animées en MarkDown, à nouveau le principe est exactement le même que pour les images normales : ![dinosaure](https://media.giphy.com/media/l3zoKeX8bMG5sMP4s/giphy.gif)

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
