## GENERATE PROTOC

### Windows

```commandline
python -m grpc_tools.protoc -I ..\protobufs --python_out=. --grpc_python_out=. ..\protobufs\recommendations.proto
```

### MAC

```commandline
python -m grpc_tools.protoc -I ../protobufs --python_out=. --grpc_python_out=. ../protobufs/recommendations.proto
```

### Local kubernetes

Deploy

```commandline
kubectl apply -f kubernetes.yml
```

Destroy

```commandline
kubectl delete -f kubernetes.yml
```
