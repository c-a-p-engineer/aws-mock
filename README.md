# Docker Amazon Web Sercice Mock

# Requirement
* [docker](https://www.docker.com/)

# Install
`.env.example` をコピー `.env` を作成。
各種設定値を修正。

Docker起動
```
docker-compose up -d --build
```

コンテナに入る
```
docker exec -it aws-cli sh
```

# Command

`--endpoint-url` は localstackを指定します。
## S3

```
aws --endpoint-url=http://localstack:4566 \
s3 mb s3://develop
```

# Note
* [localstack - docker hub](https://hub.docker.com/r/localstack/localstack)
* [localstack - github](https://github.com/localstack/localstack)

# Author
* [こぴぺたん](https://twitter.com/c_a_p_engineer)

# License
[MIT license](https://en.wikipedia.org/wiki/MIT_License).
