# Cách 1: Reset DB và sync schema, sau đó seed
npx prisma db push --force-reset && npm run seed

# Cách 2: Chỉ chạy seed (nếu schema không thay đổi)
npm run seed

Docker: npm run stack:up:build
Local dev: npm run workers:dev (không cần build)
