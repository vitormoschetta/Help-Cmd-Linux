O programa cliente SSH pode ser usado para fazer **login** em uma máquina ou servidor remoto e para **executar comandos** em uma máquina remota.


#### Acessar servidor remoto
```
ssh <user>@<server_ip_or_dns>
```
Onde:  
<user> é o nome do usuário de acesso ao servidor;  
<server_ip_or_dns> endereço IP ou DNS do servidor.  
  
<br>

#### Acessar servidor utilizando uma chave privada
```
ssh -i /<path>/<key.pem> <user>@<server_ip_or_dns>
```
Onde:  
<key.pem> deve ser substituído pelo nome do arquivo que possui a chave privada;  
<path> é o diretório que a chave privada está localizada;  
<user> idem anterior;  
<server_ip_or_dns> idem anterior.  

<br>


#### Executar comandos no servidor remoto
```
ssh user1@server1 'command1'
```
ou
```
ssh user1@server1 'command1 | command2'
```
ou
```
ssh user1@server1 "command1; command2; command3"
```
Exemplo que verifica o espaço em disco da máquina remota:
```
ssh user1@server1 'df -H'
```

#### Executar um script (varias linhas de comando)
Criar um arquivo. ex: `commands.txt` contendo os comandos um em cada linha, ex: 
```
date
df -H
```
Em seguida executar:
```
ssh user1@server1 < commands.txt
```


<https://www.cyberciti.biz/faq/unix-linux-execute-command-using-ssh/>
