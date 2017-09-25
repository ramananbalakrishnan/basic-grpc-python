# Basic gRPC in Python

Contains a minimal working example for rolling gRPC in Python.

For more details, read the accompanying [blog post](https://engineering.semantics3.com/6c4e25f0c506).

## Quickstart

```shell
git clone https://github.com/ramananbalakrishnan/basic-grpc-python
cd basic-grpc-python
pip install -r requirements.txt
python -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. calculator.proto
python server.py
python client.py
```

## File reference
```
basic-grpc-python/
├── calculator.py          # module containing a function
|
├── calculator.proto       # protobuf definition file
|
├── calculator_pb2_grpc.py # generated class for server/client
├── calculator_pb2.py      # generated class for message
|
├── server.py              # a server to expose the function
└── client.py              # a sample client
```
