
# Curl

O Curl é uma ferramenta de linha de comando utilizada para obter e enviar dados em diversos protocolos.

Seu nome provém de Client URL, que significa, URL do cliente. Ele está disponível, nativamente, na grande maioria dos sistemas operacionais baseados em Unix.

Nosso foco aqui é demonstrar os comandos mais utilizados para simular um cliente HTTP.  

Basicamente, um comando Curl é composto pela palavra curl, seguida de uma url e das opções.


## GET 
```
curl --location --request GET http://aspnetcore-dev.eba-idh62xks.us-east-1.elasticbeanstalk.com/api/product
```

<br>


## POST 
```
curl --location --request POST http://aspnetcore-dev.eba-idh62xks.us-east-1.elasticbeanstalk.com/api/product -H "Content-type: application/json" -d '{ "name": "Sardinha enlatada", "price": 5.50 }'
```


É possível referenciar um arquivo JSON para ir no corpo da requisição:
```
curl --location --request POST http://aspnetcore-dev.eba-idh62xks.us-east-1.elasticbeanstalk.com/api/product -H "Content-type: application/json" -d @content.json
```

