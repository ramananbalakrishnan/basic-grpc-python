# Basic gRPC in Python

Contains a minimal working example for getting gRPC working in Python.

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

