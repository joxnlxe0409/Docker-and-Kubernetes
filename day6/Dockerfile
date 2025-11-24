# Stage 1 — Build
FROM node:18 as builder
WORKDIR /app
COPY package*.json ./
RUN npm install

COPY . .

# Stage 2 — Run
FROM node:18-slim
WORKDIR /app

COPY --from=builder /app .

CMD ["node", "index.js"]
