# PokeApp
## Contexe:
C'est une application qui nous permet de consommer les informations sur tous les PoKémons à partir d'un API  pour afficher une liste de Pokémons avec leurs images, leurs noms, leurs types, leurs faiblesses et leurs informations de taille et de poids.
En effect la première page "MainActivity" affiche une liste déroulante des pokémons sous forme d'images avec le nom. Et la deuxième "DetailActivity" affiche les détails de chacun des pokémons cliqués.  

## Fonctionnalités:
* Affiche une liste de tous les Pokémons
* Affiche les informations détaillées d'un Pokémon sélectionné, y compris son image, son poids, sa taille, ses types et ses faiblesses.
* Utilisation de l'API REST pour récupérer les données de Pokémon

## Consommation des APIs:
La méthode  AsyncTask est utilisée pour récupérer les données des Pokémons à partir d'une URL distante. Les données sont obtenues en utilisant la classe HttpURLConnection . Cet URL contient les informations sur les Pokemons. En utilisant la méthode GET, on récupère le contenu JSON de la page qui est ensuite converti en objet JSONObject en utilisant InputStreamReader. 

## L'URL de l'API qui affiche la liste des PoKémons sous forme d'images: 
[API](https://pokeapi.co/api/v2/pokemon/) - Ce lien renvoie une liste paginée de tous les PoKémons

<img src="https://user-images.githubusercontent.com/81178741/232229365-2660560b-909f-40fc-b1fe-2b394e9062e5.jpeg" width=200>

## L'URL de l'API qui affiche les détails du PoKémon selon son {id ou nom}: 
[API/{id ou nom}](https://pokeapi.co/api/v2/pokemon/) - ajouter l'id ou le nom aprés le /

Une fois que les données sont récupérées, elles sont stockées dans une ArrayList de Pokémons et utilisées pour créer un adaptateur personnalisé (MyAdapter) qui est ensuite utilisé pour remplir la GridView. Lorsque l'utilisateur clique sur un élément de la GridView, une activité de détail (detailActivity) est lancée pour afficher des informations détaillées sur le Pokémon sélectionné.

<img src="https://user-images.githubusercontent.com/81178741/232236695-809fe475-4724-4755-9ddd-899b3da4117b.jpeg" width=200>

## Auteurs :
* ELHAJJAM Samiha: samihaelhajjam2001@gmail.com
* NHAMI Habiba: nhamihabiba@gmail.com
