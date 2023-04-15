# PokeApp
## Contexe:
C'est une application qui nous permet de consommer les informations sur tous les PoKémons à partir d'un API  pour afficher une liste de Pokémons avec leurs images, leurs noms, leurs types, leurs faiblesses et leurs informations de taille et de poids.
En effect la première page "MainActivity" affiche une liste déroulante des pokémons sous forme d'images avec le nom. Et la deuxième "DetailActivity" affiche les détails de chacun des pokémons cliqués.  

##Consommation des APIs:

HttpURLConnection est utilisé pour récupérer des données depuis une URL distante qui contient les informations sur les Pokemons en utilisant la méthode GET. 
On récupère le contenu JSON de la page qui est ensuite converti en objet JSONObject en utilisant InputStreamReader. 

## L'URL de l'API qui affiche la liste des PoKémons sous forme d'images: 
[API](https://pokeapi.co/api/v2/pokemon/) - Ce lien renvoie une liste paginée de tous les PoKémons

<img src="https://user-images.githubusercontent.com/81178741/232229365-2660560b-909f-40fc-b1fe-2b394e9062e5.jpeg" width=200>

## L'URL de l'API qui affiche les détails du PoKémon selon son {id ou nom}: 
[API/{id ou nom}](https://pokeapi.co/api/v2/pokemon/) - ajouter l'id ou le nom aprés le /

Une fois que les données sont récupérées, elles sont stockées dans une ArrayList de Pokémons et utilisées pour créer un adaptateur personnalisé (MyAdapter) qui est ensuite utilisé pour remplir la GridView. Lorsque l'utilisateur clique sur un élément de la GridView, une activité de détail (detailActivity) est lancée pour afficher des informations détaillées sur le Pokémon sélectionné.

<img src="https://user-images.githubusercontent.com/81178741/232236695-809fe475-4724-4755-9ddd-899b3da4117b.jpeg" width=200>
