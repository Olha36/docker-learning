# docker-learning
Lab5
cd frontend
npm start --->запустити додаток в режимі development
docker compose up --build
cd frontend
npm run build
npm install -g serve
serve -s build -l 3000 (побачимо мініфікований html)
cd ..
docker compose up --build
follow the link (sourcecode shall be in one link)
docker compose -f docker-compose.yml -f docker-compose.dev.yml up --build
localhost:3000 (enter in browser) (check whether it works. In react change something and see whether it changes)

