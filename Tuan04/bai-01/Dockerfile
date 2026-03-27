# Base image
FROM node:18

# Thư mục làm việc trong container
WORKDIR /app

# Copy package.json trước để cache
COPY package*.json ./

# Cài dependencies
RUN npm install

# Copy toàn bộ source code
COPY . .

# Expose port
EXPOSE 3000

# Chạy app
CMD ["npm", "start"]