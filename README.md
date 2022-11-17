# jenkinsdockergolang

main
https://github.com/agavitalis/kaniko-kubernetes

kubectl create secret docker-registry regcred --docker-server=https://index.docker.io/v1/ --docker-username=remotejob --docker-password=remotejob1Rel--docker-email=aleksander.mazurov@gmail.com
kubectl create secret generic regcred --from-file=.dockerconfigjson=/home/juno/.docker/config.json --type=kubernetes.io/dockerconfigjson


kubectl apply -f pod.yaml  #deploy on hub.docker.com
kubectl delete -f pod.yaml  
kubectl apply -f service.yaml
kubectl delete -f service.yaml

kubectl expose deployment jenkinsdockegolang-depl --type=LoadBalancer --name=jenkinsdockegolang-svc

curl http://144.21.36.80:9080
curl http://:9080

kubectl apply -f load-balancer-example.yaml
