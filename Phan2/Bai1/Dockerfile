# Sử dụng Node.js 18 làm base image
FROM node:18

# Đặt thư mục làm việc trong container
WORKDIR /app

# Copy package.json và package-lock.json (nếu có) vào container
COPY package*.json ./

# Cài đặt dependencies
RUN npm install

# Copy toàn bộ mã nguồn vào container
COPY . .

# Expose cổng 3000 để ứng dụng có thể truy cập
EXPOSE 3000

# Lệnh chạy ứng dụng khi container khởi động
CMD ["node", "index.js"]
