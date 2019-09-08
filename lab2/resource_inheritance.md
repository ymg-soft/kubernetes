Nous allons continuer de travailler avec notre cluster sur les aspects *resource limits*, 
plus avec les *namespaces* et aussi des *deployment* plus complexes. 

Nous allons utiliser un container appele *stress* que l'on va nommer *hog* .   
Verifier qu'il est bien actif.  
``kubectl create deployment hog --image systemdevformations/stress``  
et  
``kubectl get pod,deploy``  
Utilisez ``describe`` pour voir les details, il n'y a pas de limite sur l'utilisation des ressources  
``kubectl describe deployment hog``  
Obtenir la trace yaml qui a cree le deploiment  
``kubectl get deployment hog -o yaml``  
Obtenir la trace yaml sans les parametres unique dans un fichier   
``kubectl get deployment hog --export -o yaml > hog.yaml``  
Ajouter les ressources dans le fichier hog1.yaml  
Verifier avec ``describe``    
Voir la trace ``stdio`` du container  
``kubectl get po``  
``kubectl logs hog-<value>``  
Detruire le deployment  
``kubectl delete deployment hog``  
Et le recreer a nouveau   
 ``kubectl create -f hog2.yaml``  
 ``kubectl logs hog-<value>``  
Trouver le node sur lequel il fonctionne et faire un htop 