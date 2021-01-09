# Help-Cmd-Linux

### Diretório atual:
```
pwd
```

### Conteudo do Diretório:
Conteúdo diretório atual:
```
ls
```

Conteúdo subdiretórios:
```
ls -R
```

### Conteudo de um arquivo:
```
cat Startup.cs
```
Obs: Mostra no terminal o conteúdo texto do arquivo informado

### Criar novo arquivo:
```
cat > AppSettings.cs
```
Obs: Cria um arquivo com o nome _AppSettings_ de extensão _.cs_  
Atenção: Se já houver um arquivo com este nome ele substitui


### Copiar conteúdo de um arquivo para outro:
```
cat Startup.cs > NovoArquivo.cs
```
Obs: Cria um arquivo chamado _NovoArquivo_ com extensão _.cs_ com o mesmo conteúdo de _Startup.cs_


### Copiar arquivo para outro Diretório:
```
cp Program.cs Views/Home/
```
Obs: Copia o arquivo _Program.cs_ para o diretório _Views/Home/


### Converter caracteres minúsculo para maiúsculo / vice-versa:
```
cat Program.cs | tr a-z A-Z > NovoArquivo.txt
```
Obs: Cria um arquivo chamado _NovoArquivo_ com extensão _.txt com o mesmo conteúdo de _Program.cs_, porém com as letras em caixa alta.




