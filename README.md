# docker-learning
cd api
npm init -y  ---->to creat package.json
npm install express ------> to install express

At class:
npm run start + suggested link ---> to open in browser
docker build . -t real-world-docker-api
docker image ls(perhaps)
docker run -p 3001:3001 real-world-docker-api
docker ps(to see the list of containers)
docker stop + container id