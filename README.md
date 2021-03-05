# Comandos Linux



## Local

##### Saber conta de usuário logado:
```
whoami
```



##### Ver historico de comandos utilizados:
```
history 
```
###### Pesquisar um comando utilizado:
```
pressione Ctrl + R  e digite parte do texto do comando
```



##### Permissão para gravar em diretório e/ou arquivo:
```
sudo chmod a+rwx /path/
```

##### Zip arquivo:
```
zip <new_zipfile_name> <file>
```

##### Zip password:
```
zip -r --password <password> <new_zipfile> <filename>
```

##### Unzip:
```
unzip <zipfile.zip>
```



##### Efetuar dowload de arquivo:
```
wget + link
```

##### Converter caracteres minúsculo para maiúsculo / vice-versa:
```
cat Program.cs | tr a-z A-Z > NovoArquivo.txt
```

<br>


##### Localizar arquivos no Disco:
###### Localizar arquivo com nome Exato:
```
locate HomeController
```

###### Localizar arquivo com nome Aproximado:
```
locate -i Home
```

##### Localizar arquivos no Diretório / Subdiretórios :
A partir do diretório atual:
```
find . -name Program.cs
```

A partir de um diretório específico:
```
find Controllers/ -name HomeController.cs
```

##### Localizar Diretórios:
###### Será buscado diretórios/pastas com o nome _Home_:
```
find / -type d -name Home
```

##### Localizar Texto em um Arquivo:
###### Será buscado a palavra _Startup_ no arquivo _Program.cs_
###### Se o arquivo for encontrado será mostrada toda a linha onde contém a palavra pesquisada:
```
grep Startup Program.cs
```

##### Espaço em Disco
```
df -m
```

##### Comparar Diferença no conteúdo entre dois arquivos:
###### Imprime as linhas diferentes entre eles:
```
diff HomeController.cs UserController.cs
```









