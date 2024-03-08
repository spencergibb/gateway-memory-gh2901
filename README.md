# gateway-memory-gh2901

Had to add the following vm options to run `GatewayApplication`
```
-Dio.netty.tryReflectionSetAccessible=true --add-opens=java.base/java.nio=ALL-UNNAMED
```

Using oha as load testing https://github.com/hatoo/oha

```
oha -n 50000 --method POST -d helloworld http://localhost:9090/post
```