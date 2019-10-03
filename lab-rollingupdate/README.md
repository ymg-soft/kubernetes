# Rolling update
 ``k create -f frontend.yaml``  
 ``k create -f webapp-service.yaml``  
 ``chmod +x curl-test.sh``  
 `` ./curl-test.sh``  
 ``k create -f curl.yaml -n kube-public``  
 ``./curl-test.sh``
