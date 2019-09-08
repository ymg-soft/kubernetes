# Dry_run and Export 
## Commandes de base

``kubectl create deployment two --image=nginx --dry-run -o yaml`` 
il n'y a pas les informations que l'on a enlevees avant 
mais la version a apiVersion differe.  

``kubectl get deployments nginx --export -o yaml``  
ou 
``kubectl get deployments nginx --export -o json``  


 
