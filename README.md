# CinéScope

## Groupe
- Maël Roustit
- Camille Forestier

## Installation du projet
- Cloner le dépôt avec `git clone`.
- Se placer à la racine du projet et installer les dépendances avec `npm install`.
- Lancer le projet avec `npm run dev`.

## Tests d'accessibilité

### Constats
L'audit initial a mis en évidence les problèmes suivants :
- plusieurs éléments structurants étaient codés avec des `div` au lieu d'éléments HTML natifs ;
- l'étoile n'indiquait pas son rôle d'ajout ou de retrait des favoris ;
- le point rouge ou vert n'indiquait pas la disponibilité d'une séance autrement que par la couleur ;
- aucun texte n'expliquait la fonction de certains contrôles ;
- la position lors de la navigation au clavier avec `Tab` n'était pas visible ;
- la sélection d'un film n'était pas disponible au clavier.

### Corrections apportées
- Les `div` structurants ont été remplacés par des éléments HTML natifs (`header`, `nav`, `main`, `section`, `article` et `button`) afin que les technologies d'assistance puissent identifier la structure et le rôle de chaque élément.
- Les boutons de favoris disposent maintenant d'un nom accessible, d'un état `aria-pressed` et d'une infobulle.
- Les mentions « Places disponibles » et « Places indisponibles » accompagnent désormais l'indicateur coloré.
- Les contrôles disposent de libellés explicites et les affiches ont un texte alternatif.
- Un indicateur de focus visible a été ajouté pour la navigation au clavier.
- La sélection d'un film est maintenant possible avec la touche `Tab`, puis `Entrée` ou `Espace`.
