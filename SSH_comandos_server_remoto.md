O programa cliente SSH pode ser usado para fazer **login** em uma máquina ou servidor remoto e para **executar comandos** em uma máquina remota.


#### Acessar servidor remoto
```
ssh [user]@[server_ip_or_dns]
```
Onde:  
[user] é o nome do usuário de acesso ao servidor;  
[server_ip_or_dns] é o endereço IP ou DNS do servidor.  
  
<br>

#### Acessar servidor utilizando uma chave privada
```
ssh -i [path]/[key.pem] [user]@[server_ip_or_dns]
```
Onde:  
[key.pem] deve ser substituído pelo nome do arquivo que possui a chave privada;   
[path] é o diretório que a chave privada está localizada;    
[user] idem anterior;    
[server_ip_or_dns] idem anterior.    

<br>

Obs: Depois de conectado ao servidor remoto pode-se utilizar comandos bash para manipular os arquivos, diretórios e aplicações.  

<br>

#### Executar comandos diretos:
```
ssh [user]@[server_ip_or_dns] [command]
```
ou
```
ssh [user]@[server_ip_or_dns] [command01] | [command02]
```
ou
```
ssh [user]@[server_ip_or_dns] "[command01]; [command02]; [command03]"
```
<br>

Exemplo que verifica o espaço em disco da máquina remota:
```
ssh user1@server1 'df -H'
```

<br>

#### Executar um script (varias linhas de comando)
Criar um arquivo. ex: `commands.sh` contendo os comandos um em cada linha, ex: 
```
date
df -H
```
Em seguida executar:
```
ssh user1@server1 < commands.sh
```

<br>

#### Baixar arquivos de um servidor remoto:
```
scp -i [path]/[key.pem] [user]@[server_ip_or_dns]:[filename] /home/user/Downloads
```
No exemplo acima estamos baixando um arquivo [filename] existente em um servidor remoto para a pasta local de Downloads.  
Segue um exemplo pratico:
```
scp -i /opt/aws/automation.pem user@ip_or_dns:/home/user/file.txt /home/user/Downloads
```

<br>

#### Enviar / Upload de arquivos para o servidor remoto:
```
scp -i [path]/[key.pem] /home/user/[filename] [user]@[server_ip_or_dns]:[path] 
```
Segue um exemplo pratico:
```
scp -i /opt/aws/automation.pem /home/user/file.txt user@ip_or_dns:/home/user/
```

<br>
<br>

### Referências:

<https://www.cyberciti.biz/faq/unix-linux-execute-command-using-ssh/>

<http://wiki.integrator.com.br/index.php?title=Copiando_arquivos_com_SCP>

<https://www.digitalocean.com/community/tutorials/how-to-use-ssh-to-connect-to-a-remote-server-pt>
