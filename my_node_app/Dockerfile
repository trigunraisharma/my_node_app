FROM node:22.20.0-bookworm-slim
WORKDIR /app
COPY package*.json ./
RUN apt-get update && apt-get upgrade -y && apt-get clean && rm -rf /var/lib/apt/lists/*
RUN npm install
COPY . .
EXPOSE 3000
CMD ["node", "app.js"]
