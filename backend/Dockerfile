# Step 1: ベースイメージの指定
FROM docker.io/library/openjdk:17-jdk-slim

# Step 2: ワーキングディレクトリの指定
WORKDIR /app

# Step 3: Jarファイルのコピー
COPY ./target/*.jar /app/app.jar

# Step 4: コンテナが特定ポートをlistenしている事をDockerに通知
EXPOSE 8080

# Step 5: Jarファイルの実行
ENTRYPOINT ["java","-jar","app.jar"]