# Cách 1: Reset DB và sync schema, sau đó seed
npx prisma db push --force-reset && npm run seed

# Cách 2: Chỉ chạy seed (nếu schema không thay đổi)
npm run seed

###BMAD
<img width="550" height="336" alt="image" src="https://github.com/user-attachments/assets/11c4d230-b70d-4026-b5c1-9b1734fd0526" />
