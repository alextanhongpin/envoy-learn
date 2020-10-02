# Envoy example

```bash
# Starts the envoy proxy
$ docker-compose up -d

# Starts a server at port 8000
$ python3 -m http.server

# Calls the envoy listener at port 7777, which will call the cluster at port 8000.
$ curl localhost:7777
hello world
```
