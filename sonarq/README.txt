docker build -t kenlomax/sonarforjenkins:v3 .
docker push kenlomax/sonarforjenkins:v3

#docker run -9000:9000 --name jenkins --network=mynetwork kenlomax/sonarforjenkins:v1
