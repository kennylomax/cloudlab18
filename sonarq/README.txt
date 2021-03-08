docker build -t kenlomax/sonarforjenkins:v2 .
docker push kenlomax/sonarforjenkins:v2

#docker run -9000:9000 --name jenkins --network=mynetwork kenlomax/sonarforjenkins:v1
