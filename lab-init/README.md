# lab3
Build l'image kubia  
``docker build -t kubia .``
Check  
``docker images``  
Creer un container  
``docker run -d --name kubia-container -p 8080:8080 kubia``
Verifier dans votre browser 
``http://<ip_adresse>:8080``  
Voir les processes docker qui s'executent  
``docker ps``
Verifier la configuration du container  
``docker inspect kubia-container``  
Voir a l'interieur du container  
``docker exec -it kubia-container bash``
Stopper le container  
``docker stop kubia-container``  
Detruire le container  
``docker rm kubia-container``  

 



