
kubectl apply -f deployment.yml 

kubectl get pods

kubectl exec --stdin --tty cloudlab18sonardeployment-5848ccd78c-7gxbz   -- /bin/bash

curl "http://admin:admin@cloudlab18sonarservice:9000/api/qualitygates/set_as_default" -X POST -d  "name=myqualitygate"



curl "http://admin:admin@cloudlab18service:9000/api/qualitygates/set_as_default" -X POST -d  "name=myqualitygate"

