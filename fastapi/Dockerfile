FROM python:3.12

# 環境変数設定
ENV PYTHONUNBUFFERED=1 \
    PIP_NO_CACHE_DIR=1 \
    PIP_DISABLE_PIP_VERSION_CHECK=1

# 作業ディレクトリを設定
WORKDIR /app

# 依存関係をコピーしてインストール
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# アプリケーションのコードをコピー
COPY . .

CMD ["python", "main.py"]
