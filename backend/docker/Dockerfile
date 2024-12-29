# Pythonバージョン設定
FROM python:3.12

# 作業ディレクトリの設定
WORKDIR /app

# 依存関係をコピー
COPY ../requirements.txt /app/

# 必要なパッケージをインストール
RUN pip install --no-cache-dir -r requirements.txt

# アプリケーションファイルのコピー
COPY .. /app/

# サーバー起動コマンド
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

