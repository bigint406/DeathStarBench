```
helm install dsb-mm . -n dsb-mm --set-string global.imagePullPolicy="IfNotPresent"
```

配置文件地址改成了gitee，sb开发者用git clone拿配置文件

```
python3 scripts/write_movie_info.py -c <path-to-casts.json> -m <path-to-movies.json> --server_address <address:port> && scripts/register_users.sh && scripts/register_movies.sh
```