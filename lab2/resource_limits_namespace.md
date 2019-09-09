# Resources_limits_namespace

## Basic commands

Creez un nouveau namespace appele ``low-usage-limit`` et verifiez    
``kubectl create namespace low-usage-limit``  
``kubectl get namespace``  
Utiliser le fichier low-resource-range.yaml et l'integrer au namespace  
``kubectl --namespace=low-usage-limit create -f low-resource-range.yaml`` 
Utilisation du namespace pour creer un deploiement  
``kubectl create -n low-usage-limit deployment limited-hog --image systemdevformations/stress``  
Verifier    
 ``kubectl get LimitRange``  
Attention il faut specifier le namespace  
``kubectl -n low-usage-limit get LimitRange``  
``kubectl get deployments --all-namespaces``  
 