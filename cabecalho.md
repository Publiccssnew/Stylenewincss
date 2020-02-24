Gerar cabeçalho padronizado para arquivos de códigos fonte 
de programas com nome do programa, autor, data, email, etc.

.SH RESUMO
.B cabecalho
[\-h] [\-\-help] [-v] [\-\-version] [\-\-config] [\-\-list] 
[\-sh] [\-sci] [\-c] [\-c++] [\-tex] [\-py] [\-f90] [\-mf90] [\-html] [\-js]
[\-css] [\-java] [\-php] [\-html\-php] [\-m]

.SH DESCRIÇÃO
.PP
CABECALHO é um auxiliar para gerar a documentação dos seus programas.
Ao utilizar este programa você pode estabelecer um cabeçalho padrão para
a maioria das linguagens de programação que for trabalhar.

.SH OPÇÕES
CABECALHO aceita as seguintes opções:
.TP 8
.B  \-h, \-\-help
Exibe a mensagem de ajuda do programa e sai.
.TP 8
.B \-v, \-\-version
Exibe a versão do programa.
.TP 8
.B \-\-config
Configura variáveis de ambiente do programa cabecalho, 
como o nome do programador e email a serem exibidos no cabeçalho 
do programa, por exemplo. Utilizando a sintaxe \fBvariável=valor\fP.
.TP 8
.B \-\-list
Lista todas as variáveis de ambiente já definidas para o programa.
.TP 8
.B \-sh
Gerar cabeçalho para um programa em shell script.
.TP 8
.B \-sci 
Gerar cabeçalho para um programa do scilab.
.TP 8
.B \-c
Gerar cabeçalho para um programa em C.
.TP 8
.B \-c++
Gerar cabeçalho para um programa em C++.
.TP 8
.B \-tex
Gerar cabeçalho LaTeX.
.TP 8
.B \-py
Gera cabeçalho Python.
.TP 8
.B \-f90
Gerar cabeçalho Fortran 90.
.TP 8
.B \-mf90
Gerar cabeçalho Módulo Fortran 90.
.TP 8
.B \-html
Gerar cabeçalho de página HTML.
.TP 8
.B \-js
Gerar cabeçalho de arquivo JavaScript.
.TP 8
.B \-css
Gerar cabeçalho para folha de estilo CSS.
.TP 8
.B \-java
Gerar cabeçalho para arquivo classe Java.
.TP 8
.B \-php
Gerar cabeçalho para arquivo de script PHP.
.TP 8
.B \-html\-php
Gerar cabeçalho de Página HTML com PHP.
.TP 8
.B \-m <objetivo>
Acrescentar <objetivo> ao Objetivo no cabeçalho do arquivo.

.SH EXEMPLOS DE USO
.PP
Gerar arquivo .sh (Shell Script) com cabeçalho (Documentação).

	~$ cabecalho -sh Arquivo.sh
.PP
Gerar cabeçalho com o objetivo do programa definido (Use aspas duplas).

	~$ cabecalho -sh Arquivo.sh -m "Objetivo para este programa"
.PP
Configurar o nome do programador para utilizar em todos os cabeçalhos (Use aspas duplas).

	~$ cabecalho --config user.programador="Rodolfo Dirack"
[Para mais detalhes consulte os manuais de uso dos programas desta biblioteca](https://github.com/Dirack/Shellinclude/blob/master/manuais).