#### Instalação:
``` 
apt-get install vim
```


#### Abrir um arquivo:
``` 
vi file.txt
```

<br>

#### Modo inserção/edição:
Apenas pressione a tecla `i`

<br>

#### Salvar alterações e sair:
Pressione a tecla `Esc` e em seguida digite:
``` 
:wq
```

<br>

#### Excluir todo o contedo do arquivo:
Pressione a tecla `Esc` e em seguida digite:
``` 
:1,$d
```

ou, estando na última linha do arquivo, digitar:
``` 
dggg
```

<br>

#### Navegar para o início do arquivo (primeiro caractere, primeira linha):
Pressione duas vezes a tela `g` no modo de comando
``` 
gg
```

<br>

#### Sair sem salvar:
``` 
:q!
```

<br>

#### Buscar e substituir:
``` 
:%s/texto/novo_texto
```

<br>

#### Buscar e substituir (ser avisado em cada item se deseja realmente substituir):
``` 
:%s/texto/novo_texto/gc
```
Opções:
    y: sim
    n: não
    a: substituir tudo
    q: sair
    l: substitua esta ocorrência e saia
    ^ E (Ctrl + E) : Rolar uma tela para cima
    ^ Y (Ctrl + Y) : Rola uma tela para baixo


<br>


#### Help:
``` 
:help
```

<br>
