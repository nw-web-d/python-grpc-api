## 環境構築

* python3インストール（略
* 関連モジュールインストール
```
pip install grpcio
pip install grpcio-tools
```

## generate gRPC code

```
python3 -m grpc_tools.protoc -I./protos --python_out=. --grpc_python_out=. ./protos/helloworld.proto
```


## RUN

```
python3 greeter_server.py
```