Le "full-text search" (recherche textuelle intégrale) est une fonctionnalité qui permet de rechercher des données textuelles dans une base de données de manière plus flexible que la simple égalité de chaînes de caractères. Cette fonctionnalité est souvent utilisée pour rechercher des mots ou des phrases dans de grandes quantités de texte, comme des articles, des documents ou des descriptions de produits.

Avec JSON Server, le "full-text search" peut être simulé en utilisant l'opérateur _q. Cet opérateur permet de rechercher une chaîne de caractères dans toutes les propriétés des objets JSON.

Par exemple, supposons que vous avez un ensemble de données contenant des articles, et vous souhaitez rechercher tous les articles contenant le mot "JavaScript" dans leur titre ou leur contenu. Vous pouvez envoyer une requête GET à votre serveur JSON Server avec l'opérateur _q :

http://localhost:3000/data?_q=JavaScript


Cette requête retournera tous les éléments où le mot "JavaScript" apparaît dans n'importe quelle propriété. Le "full-text search" avec l'opérateur _q est utile pour effectuer des recherches flexibles sur des données textuelles sans avoir besoin de spécifier explicitement les propriétés dans lesquelles effectuer la recherche. Cependant, il est à noter que cette fonctionnalité peut ne pas être aussi sophistiquée qu'un moteur de recherche textuelle complet, mais elle fournit une fonctionnalité de recherche de base qui peut être très pratique pour de nombreuses applications.