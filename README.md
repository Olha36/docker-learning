﻿# docker-learning
Lab8 <br /> 
az login --use-device-code<br /> 
az group create --name OlhaKResourceGroup --location eastus<br /> 
("name": "OlhaKResourceGroup",) <br /> 
az acr create --resource-group OlhaKResourceGroup --name olhakucherukregistry  --sku Basic <br /> 
("loginServer": "olhakucherukregistry.azurecr.io",) <br /> 
az acr login --name olhakucherukregistry <br /> 
git clone https://github.com/Azure-Samples/azure-voting-app-redis.git ---> creating container <br /> 
cd azure-voting-app-redis ---> enter the folder <br /> 
//Run multi-container application locally: <br /> 
docker-compose up --build -d <br /> 
docker images ---> to see created images <br /> 
http://localhost:80 ---> see the running application <br /> 
docker-compose down ---> stop the application <br /> 
docker-compose push ---> send  images on azure <br /> 
docker login azure <br /> 
docker context create aci myacicontext <br /> 
choose resoursegroup (OlhaKResourceGroup) <br /> 
docker context use myacicontext <br /> 
docker compose up(розгортає проект) <br /> 
docker ps (copy port and paste in the browser) <br /> 

