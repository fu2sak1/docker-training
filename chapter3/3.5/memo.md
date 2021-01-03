# 3.5

- Serviceはレプリカ数（コンテナの数）を制御することで容易にコンテナを複製でき、複数のノードに配置できるためスケールアウトへの親和性が高い
- Serviceによって管理される複数のレプリカはService名で名前解決でき、かつServiceへのトラフィックはレプリカに分散される
- Swarmクラスタの外からSwarmのServiceを利用するには、Serviceにトラフィックを分散するためのプロキシを用意する
- Stackは複数のServiceをグルーピングでき、複数のServiceで形成されるアプリケーションのデプロイに役立つ

## サービスの作成

```cmd
docker service create [OPTIONS] IMAGE [COMMAND] [ARG...]
```

## サービスの削除

```cmd
docker service rm SERVICE [SERVICE...]
```
