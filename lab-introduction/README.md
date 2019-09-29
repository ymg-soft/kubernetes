# Lab introduction 
# Basic commands  
Creer un pod avec un fichier YAML  
``kubectl create -f pod-definition.yaml``  
Verifier  
``kubectl get pods``  
``kubectl describe pod myapp-pod``  

Comment gerer du code yaml  
``kubectl run --generator=run-pod/v1 nginx --image=nginx --dry-run -o yaml``
