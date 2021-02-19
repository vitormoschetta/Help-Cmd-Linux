## Comandos Linux

##### Saber conta de usuário logado:
```
whoami
```

##### Saber o diretório atual:
```
pwd
```

##### Conteudo do diretório:
```
ls
```
###### Conteudo do diretório em lista:
```
ls -l
```
###### Conteudo do diretório em lista + ocultos (aqui vc encontra o arquivo .ssh que é as chaves utilizadas nos repositórios remotos)
```
ls -la
```

##### Entrar em um diretório:
```
cd Desktop
```

##### Sair de um diretório:
```
cd ../
```

##### Ir para o diretório home/user:
```
cd ~
``` 

##### Navegar p um diretório a partir do home/user:
```
cd ~/Documents
```

##### Navegar p o diretório raiz:
```
cd /
```


##### Ver historico de comandos utilizados:
```
history 
```
###### Pesquisar um comando utilizado:
```
pressione Ctrl + R  e digite parte do texto do comando
```

##### Criar uma pasta:
```
mkdir nome_pasta
```

##### Excluir arquivo ou pasta vazia:
```
rmdir nome_pasta
```

##### Excluir diretório inteiro:
```
rm -r diretorio
```

##### Criar arquivo texto:
```
cat > arq.txt
```

##### Conteudo de um arquivo:
```
cat Startup.cs
```

##### Copiar conteúdo de um arquivo para outro:
```
cat Startup.cs > NovoArquivo.cs
```

##### Mover arquivo para outro Diretório:
```
mv Program.cs Views/Home/
```

##### Renomear arquivo:
```
mv AppSettings.cs Settings.cs
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









