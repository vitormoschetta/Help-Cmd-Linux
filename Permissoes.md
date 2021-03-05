# Permissões



##### Define as permisses para gravar em diretório e/ou arquivo:
```
sudo chmod a+rwx /path/
```

- r = leitura.
- w = gravação.
- x = execução (para arquivos) ou autorização de acesso (para diretórios).

<br>

##### Define o proprietário (owner) do arquivo:
```
sudo chown vfarias <file_name>
```

<br>

##### Verifica permissões e proprietário do arquivo:
```
ls -l teste.txt
```
  
  saída:   
    -rw-r--r-- 1 vfarias vfarias 11 mar  5 15:09 teste.txt



<br>
<br>

##### Referências:

<https://askubuntu.com/questions/918379/what-is-the-main-difference-between-chmod-and-chown>
