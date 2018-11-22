
#start (using Powershell)
1. cd C:\Projects\deployment-pipeline-aspdotnet-core-docker
2. cd registry
    docker-compose up -d
    cd ..

3. cd teamcity
    docker-compose up -d
    cd ..


#urls

1. registry
http://localhost:55000

2. teamcity server
http://localhost:8111


#push image to registry my-registry:55000
docker tag aspnetcore/generator:multi my-registry:55000/aspnetcore/generator:multi
docker push my-registry:55000/aspnetcore/generator:multi
