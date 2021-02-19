# Help-Cmd-Linux

Trabalhando com a linha de comando do linux. 


<br>

Saber o diretório atual:
```
pwd
```


<br>

Conteudo do diretório:
```
ls
```


<br>

Conteúdo subdiretórios:
```
ls -R
```


<br>


### Conteudo de um arquivo:
```
cat Startup.cs
```
> Mostra no terminal o conteúdo texto do arquivo informado
<br>


### Criar novo arquivo:
```
cat > AppSettings.cs
```
> Cria um arquivo com o nome _AppSettings_ de extensão _.cs_  
> Atenção: Se já houver um arquivo com este nome ele substitui
<br>


### Copiar conteúdo de um arquivo para outro:
```
cat Startup.cs > NovoArquivo.cs
```
> Cria um arquivo chamado _NovoArquivo_ com extensão _.cs_ com o mesmo conteúdo de _Startup.cs_
<br>


### Copiar arquivo para outro Diretório:
```
cp Program.cs Views/Home/
```
> Copia o arquivo _Program.cs_ para o diretório _Views/Home/
<br>


### Mover arquivo para outro Diretório:
```
mv Program.cs Views/Home/
```
> Move o arquivo _Program.cs_ para o diretório _Views/Home/
<br>


### Renomear arquivo:
```
mv AppSettings.cs Settings.cs
```
> Renomeia AppSettings.cs_ para _Settings.cs_
<br>


### Criar novo Diretório:
```
mkdir Configurations/JWT
```
<br>


### Excluir Diretório / Arquivo
Excluir Diretório Vazio:
```
rmdir Configurations
```
> Só funciona se o diretório _Configurations_ estiver vazio
<br>

Excluir Arquivo de um Diretório:
```
rmdir Configurations/JWT/arquivo.txt
```
> Irá excluir o _arquivo.txt_
<br>

Excluir todo conteúdo de um Diretório:
```
rm -r Configurations
```
> Atençao: Cuidado, pois não há mensagem de confirmação.
<br>


### Localizar arquivos no Disco:
Localizar arquivo com nome Exato:
```
locate HomeController
```
> É _case-sensitive_, ou seja, diferencia letras maiúsclas de minúsculas
<br>

Localizar arquivo com nome Aproximado:
```
locate -i Home
```
> Não é _case-sensitive_
> Irá imprimir no console todas as linhas de arquivos que possuem a palavra Home
<br>


### Localizar arquivos no Diretório / Subdiretórios :
A partir do diretório atual:
```
find . -name Program.cs
```
<br>

A partir de um diretório específico:
```
find Controllers/ -name HomeController.cs
```
<br>


### Localizar Diretórios:
```
find / -type d -name Home
```
> Será buscado diretórios/pastas com o nome _Home_
<br>


### Localizar Texto em um Arquivo:
```
grep Startup Program.cs
```
> Será buscado a palavra _Startup_ no arquivo _Program.cs_
> Se o arquivo for encontrado será mostrada toda a linha onde contém a palavra pesquisada.
<br>


### Espaço em Disco
```
df -m
```
<br>


### Comparar Diferença no conteúdo entre dois arquivos:
```
diff HomeController.cs UserController.cs
```
> Imprime as linhas diferentes entre eles
<br>


### Efetuar dowload de arquivo:
```
wget + link
```
<br>


### Ver historico de comandos utilizados:
```
history 
```
<br>


### Converter caracteres minúsculo para maiúsculo / vice-versa:
```
cat Program.cs | tr a-z A-Z > NovoArquivo.txt
```
> Cria um arquivo chamado _NovoArquivo_ com extensão _.txt com o mesmo conteúdo de _Program.cs_, porém com as letras em caixa alta.






