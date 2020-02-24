#### Fazer backup de um arquivo ou de uma lista de arquivos em um arquivo zipado na pasta atual

BACKUP é uma interface em shell para o programa 'tar' nativo do unix. 

#### RESUMO DAS OPÇÕES

[\-h] [\-\-help] [-v] [\-\-version] [\-a]
[\-l] [\-\-list]

#### DESCRIÇÃO DAS OPÇÕES

\-h, \-\-help
Exibe a mensagem de ajuda do programa e sai.

\-v, \-\-version
Exibe a versão do programa e sai.

\-a
Faz o backup de arquivo fornecido pelo usuário.

\-l, \-\-list
Faz o backup de uma lista de arquivos fornecidos ao programa 
em um arquivo de texto.

#### EXEMPLOS DE USO

* Fazer backup de 'arquivo.txt'.

```sh
~$ backup -a arquivo.txt 
```

* Fazer backup de mais de um arquivo.

```sh
~$ backup -a arq1.txt arq2.txt arq3.txt
```

* Fazer backup de uma lista de arquivos.

```sh
~$ backup -l lista.txt
```

[Para mais detalhes consulte os manuais de uso dos programas desta biblioteca](https://github.com/Dirack/Shellinclude/blob/master/manuais).