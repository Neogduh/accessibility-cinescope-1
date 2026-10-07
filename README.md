# Here starts the journey with Cinescope

## Groupe
- Maël Roustit
- Camille Forestier

## First install your project
- you can copy the repo locally using `git clone`
- go to the root of the directory and run `npm i`
- run the project with `npm run dev`

## Now it's time to test it

### Constats
- Les éléments sont codés avec des `div` au lieu d'éléments HTML natifs.
- L'étoile n'indique pas son rôle (probablement l'ajout aux favoris).
- Le point rouge/vert n'indique pas sa signification (probablement la disponibilité d'une séance).
- Au survol, aucun texte n'explique la fonction des éléments.
- Lors de la navigation au clavier avec `Tab`, la position sur la page n'est pas visible.
- La fonctionnalité de sélection de film lorsqu'on clique dessus n'est pas disponible au clavier.

### Justification de la correction de 3 éléments
- Nous avons remplacé les `div` par des éléments HTML natifs (`header`, `nav`, `main`, `button`, etc.) afin que les technologies d'assistance puissent identifier la structure et le rôle de chaque élément.
- Nous avons ajouté, à côté du point rouge/vert, le texte "Places disponibles" ou "Places indisponibles" afin d'expliciter sa signification sans reposer uniquement sur la couleur.
- Nous avons ajouté un indicateur de focus visible afin que l'utilisateur repère sa position sur la page lors de la navigation au clavier.
