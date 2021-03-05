# Permissões



#### Define as permisses para gravar em diretório e/ou arquivo:
```
sudo chmod a+rwx /path/
```

- r = leitura.
- w = gravação.
- x = execução (para arquivos) ou autorização de acesso (para diretórios).

<br>

#### Define o proprietário (owner) do arquivo:
```
sudo chown vfarias <file_name>
```

<br>

#### Verifica permissões e proprietário do arquivo:
```
ls -l teste.txt
```
  
    saída:   
    
      -rw-r--r-- 1 vitor admins 11 mar  5 15:09 teste.txt

A saída acima, informa que o arquivo `teste.txt` é de propriedade do usuario **vitor** e pertence ao grupo **admins**


<br>

Vamos seguir vendo outros exemplos:

```
chmod ug+rw teste.txt
```
Define que o arquivo teste.txt pode ser lido (**r**) e alterado (**w**) pelo dono (**u**) e pelos usuários que são membros do mesmo grupo (**g**) do arquivo teste.txt

<br>
<br>

##### Referências:

<https://askubuntu.com/questions/918379/what-is-the-main-difference-between-chmod-and-chown>
