# ==== CONFIGURE =====
# Use a Node 18 base image
FROM node:18-alpine AS builder
ENV NODE_ENV development
WORKDIR /app
# Copy app files
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
# Expose the port on which the app will be running (3000 is the default that `serve` uses)
EXPOSE 3000