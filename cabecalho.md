#### Gerar cabeçalho padronizado para arquivos de códigos fonte de programas

CABECALHO  é  um  auxiliar  para gerar a documentação dos seus programas.  Ao utilizar
este programa você pode estabelecer um cabeçalho padrão para a maioria das  linguagens
de programação que for trabalhar.


#### RESUMO DAS OPÇÕES
[\-h] [\-\-help] [-v] [\-\-version] [\-\-config] [\-\-list] 
[\-sh] [\-sci] [\-c] [\-c++] [\-tex] [\-py] [\-f90] [\-mf90] [\-html] [\-js]
[\-css] [\-java] [\-php] [\-html\-php] [\-m]

#### DESCRIÇÃO DAS OPÇÕES

\-h, \-\-help
Exibe a mensagem de ajuda do programa e sai.

\-v, \-\-version
Exibe a versão do programa.

\-\-config
Configura variáveis de ambiente do programa cabecalho, 
como o nome do programador e email a serem exibidos no cabeçalho 
do programa, por exemplo. Utilizando a sintaxe \fBvariável=valor\fP.

\-\-list
Lista todas as variáveis de ambiente já definidas para o programa.

\-sh
Gerar cabeçalho para um programa em shell script.

\-sci 
Gerar cabeçalho para um programa do scilab.

\-c
Gerar cabeçalho para um programa em C.

\-c++
Gerar cabeçalho para um programa em C++.

\-tex
Gerar cabeçalho LaTeX.

\-py
Gera cabeçalho Python.

\-f90
Gerar cabeçalho Fortran 90.

\-mf90
Gerar cabeçalho Módulo Fortran 90.

\-html
Gerar cabeçalho de página HTML.

\-js
Gerar cabeçalho de arquivo JavaScript.

\-css
Gerar cabeçalho para folha de estilo CSS.

\-java
Gerar cabeçalho para arquivo classe Java.

\-php
Gerar cabeçalho para arquivo de script PHP.

\-html\-php
Gerar cabeçalho de Página HTML com PHP.

\-m <objetivo>
Acrescentar <objetivo> ao Objetivo no cabeçalho do arquivo.

#### EXEMPLOS DE USO

* Gerar arquivo .sh (Shell Script) com cabeçalho (Documentação).

```sh
~$ cabecalho -sh Arquivo.sh
```

* Gerar cabeçalho com o objetivo do programa definido (Use aspas duplas).

```sh
~$ cabecalho -sh Arquivo.sh -m "Objetivo para este programa"
```

* Configurar o nome do programador para utilizar em todos os cabeçalhos (Use aspas duplas).

```sh
~$ cabecalho --config user.programador="Rodolfo Dirack"
```

[Para mais detalhes consulte os manuais de uso dos programas desta biblioteca](https://github.com/Dirack/Shellinclude/blob/master/manuais).