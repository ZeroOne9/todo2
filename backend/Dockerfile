FROM node:20-alpine

# Tạo thư mục app
WORKDIR /app

# Copy package trước để tận dụng cache
COPY package*.json ./

# Cài dependencies
RUN npm install

# Copy toàn bộ source
COPY . .

# Expose port backend
EXPOSE 4000

# Start server
CMD ["npm", "run", "dev"]
