# docker-learning
Lab8
az login --use-device-code
az group create --name OlhaKResourceGroup --location eastus
("name": "OlhaKResourceGroup",)
az acr create --resource-group OlhaKResourceGroup --name olhakucherukregistry  --sku Basic
("loginServer": "olhakucherukregistry.azurecr.io",)
az acr login --name mycontainerregistry082
git clone https://github.com/Azure-Samples/azure-voting-app-redis.git ---> creating container
cd azure-voting-app-redis ---> enter the folder
//Run multi-container application locally:
docker-compose up --build -d
docker images ---> to see created images
http://localhost:80 ---> see the running application
docker-compose down ---> stop the application
docker-compose push ---> send  images on azure
docker login azure
docker context create aci myacicontext
choose resoursegroup (OlhaKResourceGroup)
docker context use myacicontext
docker compose up(розгортає проект)
docker ps (copy port and paste in the browser)

