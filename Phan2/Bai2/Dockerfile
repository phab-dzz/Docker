# Sử dụng Python 3.9 làm base image
FROM python:3.9

# Đặt thư mục làm việc trong container
WORKDIR /app

# Copy các file vào container
COPY requirements.txt .
COPY app.py .

# Cài đặt thư viện
RUN pip install --no-cache-dir -r requirements.txt

# Expose cổng 5000 để truy cập ứng dụng
EXPOSE 5000

# Chạy ứng dụng Flask
CMD ["python", "app.py"]
