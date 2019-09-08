# Expose
## Commandes de base

``kubectl expose deployment/nginx``   
 

Pour modifier une configuration existante dans un cluster, vous pouvez utiliser des 
sous-commandes **apply**, **edit** ou **patch** pour un correctif sans arret du pod.  
La commande **apply** effectue un diff entre les precedentes modifications, 
la version actuelle et les modifications en cours, les champs non mentionnés ne sont pas affectés.   
**Edit** effectue un get, ouvre un éditeur, puis applique les modifications.  
Vous pouvez mettre à jour des objets API  avec **patch** JSON et la fonctionnalité de correctif de fusion ou de correctif de fusion stratégique.  
Si la configuration comporte des champs *ressource* qui ne peuvent pas être mis à jour une fois initialisés, une mise à jour "forcée" peut être effectuée.
en utilisant l'option ``replace --force``. Cela supprime d'abord, puis recrée une ressource.


``kubectl replace -f second_with_expose.yaml``  
 
