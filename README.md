# docker-learning
Lab6
docker compose -f docker-compose.yml -f docker-compose.dev.yml up --build
localhost 3000 (код не мініфікований) (працює в режимі розробки)
docker compose up --build (подивитися, як працює в режимі продакшн. Код має стати мініфікованим)
real-world-docker.dev ---> check
docker compose up --build --> test api(real-world-docker.dev/api/)
docker compose -f docker-compose.yml -f docker-compose.dev.yml up --build --> запустити в режимі девелопмента
real-world-docker.dev ---> check
real-world-docker.dev/api
docker logs + container ---> api address
docker system prune --all ---> to clean docker(видаляє образи, контейнери, чистить кеш)

