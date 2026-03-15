FROM python:3.11-slim

WORKDIR /app

# 必要なライブラリがあればここに書く（今は最小限）
RUN pip install --no-cache-dir pandas matplotlib

COPY . .

CMD ["python", "--version"]