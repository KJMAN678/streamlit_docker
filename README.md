## Docker コマンド

```
# フォルダの変更
cd streamlit_docker

# ローカルの Dockerfile から Docker イメージ作成
docker build .

# Docker イメージの一覧確認
docker images

# Docker イメージに名前とタグを付ける
docker tag [イメージID] xxx/xxx:[バージョンの数値]

# Docker コンテナの起動
docker run -i -t -p 8501:8501 --name [コンテナ名] xxx/xxx:[バージョンの数値]

# 起動中のコンテナ一覧を表示
docker ps

# 休止中のコンテナ一覧を表示
docker ps -a

# Docker コンテナの停止
docker stop [コンテナID]

# Docker コンテナの削除
docker rm [コンテナID]

# Docker イメージの削除
docker rmi [イメージID]
```

ローカルサーバーのアドレス  
http://localhost:8501/  

![0397f2dad11c5d3cb0ca30a6b46d34b3](https://user-images.githubusercontent.com/45703844/166457963-b8faae81-075b-4ea3-a306-4fa994a5dbbf.png)

## 参考サイト
- [Python: Streamlit を使って手早く WebUI 付きのプロトタイプを作る](https://blog.amedama.jp/entry/streamlit-tutorial)  
- [Deploy a Streamlit Web App with Azure App Service](https://towardsdatascience.com/deploying-a-streamlit-web-app-with-azure-app-service-1f09a2159743)  
- [公式ドキュメント Docker Build](https://docs.docker.jp/engine/reference/commandline/build.html)  
- [公式ドキュメント Docker Tag](https://docs.docker.jp/engine/reference/commandline/tag.html)  
- [Docker + ローカルサーバーでの起動時の留意点](https://web.plus-idea.net/on/docker-web-server-access-denied/)  