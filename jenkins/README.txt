docker build -t kenlomax/jenkinsforsonar:v4 .
docker push kenlomax/jenkinsforsonar:v4


#docker run -p8080:8080 --name sonarqube  --network=mynetwork kenlomax/jenkinsforsonar:v1
