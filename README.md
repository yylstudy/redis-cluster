基于

cluster-announce-ip

cluster-announce-port

cluster-announce-bus-port

三个参数来在构建一个在供外部访问的redis集群，访问方式为vip+NodePort

部署：   
在部署redis节点上增加deploy-redis=true label   
kubectl label nodes 10.100.243.3 deploy-redis=true   
helm install redis-cluster .

