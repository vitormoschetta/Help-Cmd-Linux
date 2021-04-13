
## Teste de Conexão


### Telnet
```
telnet <hostname> <port>
```

##### Exemplo:
```
telnet google.com 80
```
Saída com sucesso:
```
Trying 172.217.173.110...
Connected to google.com.
```




### cUrl
```
curl -v telnet://<hostname>:<port>
```

##### Exemplo:
```
curl -v telnet://google.com:80
```
Saída com sucesso:
```
Rebuilt URL to: telnet://google.com:80/
*   Trying 172.217.173.110...
* TCP_NODELAY set
* Connected to google.com (172.217.173.110) port 80 (#0)

```
