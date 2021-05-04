
# Curl

O que é Comando Curl? É um comando disponível na maioria dos sistemas baseado em Unix. Ele é usado como abreviação para “Client URL”. Comandos Curl são destinados para funcionar como uma forma de verificar a conectividade da URL, além de ser uma ótima ferramenta de transferência de dados. 

O Comando Curl suporta a lista de protocolos abaixo:

    HTTP e HTTPS;
    FTP e FTPS;
    IMAP e IMAPS;
    POP3 e POP3S;
    SMB e SMBS;
    SFTP;
    SCP;
    TELNET;
    GOPHER;
    LDAP e LDAPS;
    SMTP e SMTPS.
    
Para saber a versão instalada e os protocolos aceitos pela versão:
```
curl --version
```

Nosso foco aqui é demonstrar os comandos mais utilizados para simular um cliente HTTP:

```
curl https://www.google.com/
```
A requisição acima vai imprimir no console o HTML da página do Google.  

Podemos também salvar esse conteúdo em um arquivo específico:
```
curl -o file.html https://www.google.com/
```


## GET 
```
curl --location --request GET http://aspnetcore-dev.eba-idh62xks.us-east-1.elasticbeanstalk.com/api/product
```

<br>


## POST 
```
curl --location --request POST http://aspnetcore-dev.eba-idh62xks.us-east-1.elasticbeanstalk.com/api/product \ 
-H "Content-type: application/json" -d '{ "name": "Sardinha enlatada", "price": 5.50 }'
```


É possível referenciar um arquivo JSON para ir no corpo da requisição:
```
curl --location --request POST http://aspnetcore-dev.eba-idh62xks.us-east-1.elasticbeanstalk.com/api/product \ 
-H "Content-type: application/json" -d @files/content.json
```



<br>
<br>

### Referências

<https://devcontent.com.br/artigos/linux/lista-de-comandos-curl>

<https://www.hostinger.com.br/tutoriais/comando-curl-linux>
