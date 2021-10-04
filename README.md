# Solution "point de vente" pour hôtels

Le système est composé d'une **application Android** (React Native) et d'une **interface web** de gestion (Laravel/PHP). L'application est utilisée par la réception d'un hotel pour enregistrer les ventes (chambres et autres produits), les paiements, les remboursements, etc. L'interface web permet de visualiser et d'exporter les opérations, et d'éditer les produits disponibles.

Le système a été développé pour un client spécifique selon ses besoins et son budget. Le client utilise d'ailleurs le système depuis plus de quatre ans sans problèmes.

L'application Android, développée en JavaScript avec React Native devait être simple d'utilisation et pouvoir permettre de continuer les opérations même si elle devait être temporairement déconnectée de l'Internet. Un historique des transactions est gardé en mémoire et une synchronisation s'effectue lorsque l'appareil se connecte à l'Internet. L'application permet également la modification de ventes passées (pour ajouter un remboursement, par exemple) et le système supporte plusieurs applications utilisées concurremment.

Une API web permet à l'application de mettre à jour les commandes et de récupérer les nouvelles informations (comme des changements de prix).

L'interface de gestion web permet d'accéder aux ventes enregistrées depuis l'application et de mettre à jour la liste des produits. Le système supporte également l'attribution de taxes aux produits.

Modules
---

* `tabletui` : [l'application Android](https://github.com/xfrenette/hotelcaisse-tabletui), en React Native.
* `jsapp` : [la librairie JavaScript](https://github.com/xfrenette/hotelcaisse-jsapp), utilisée par `tabletui`.
* `server` : [le serveur web (API et outil de gestion)](https://github.com/xfrenette/hotelcaisse-server), programmé avec PHP et Laravel.