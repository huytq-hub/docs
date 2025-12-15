# Cách 1: Reset DB và sync schema, sau đó seed
npx prisma db push --force-reset && npm run seed

# Cách 2: Chỉ chạy seed (nếu schema không thay đổi)
npm run seed

Docker: npm run stack:up:build

Local dev: npm run workers:dev (không cần build)



Build TypeScript code: npm run workers:build

Rebuild Docker image: docker compose -f infra/docker-compose.yml build workers

Restart container: docker compose -f infra/docker-compose.yml up -d workers

rebuild và restart: docker compose -f infra/docker-compose.yml up --build -d workers

docker logs -f ondo-workers


# Từ thư mục infra
docker compose -f docker-compose.yml build workers

# Hoặc từ root project
docker compose -f infra/docker-compose.yml build workers

# Hoặc rebuild và restart
docker compose -f infra/docker-compose.yml up --build -d workers
