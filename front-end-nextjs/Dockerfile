FROM node:18-alpine AS base

WORKDIR /app

COPY package.json yarn.lock* package-lock.json* pnpm-lock.yaml* ./

RUN \
  if [-f yarn]

COPY . .

RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]
