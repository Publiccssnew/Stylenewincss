#### Compila e instala programas escritos em linguagem C na sua cópia local do pacote de processamento sísmico MADAGASCAR.

COMP é um auxiliar para a compilação e instalação de programas no MADAGASCAR.
Por padrão o MADAGASCAR instala o pacote em um diretório identificado pela
variável de ambiente $RSFROOT configurada no momento da instalação. E mantém
a cópia local dos arquivos e códigos fonte no diretório em $RSFSRC.

Assim, para adicionar novos programas à sua cópia local do MADAGASCAR. Basta
adicionar os seus programas em $RSFSRC/user/<seuDiretorio> com o script SConstruct
de instalação e rodar o 'comp -c <seuDiretorio>'. O programa irá procurar pelo
seu diretório em $RSFSRC, rodar o SConstruct de compilação e depois rodar
o comando 'scons install' em $RSFSRC.

Consulte a documentação oficial no site do Madagascar para saber como 
[adicionar programas ao pacote madagascar](http://www.ahay.org/wiki/Adding_new_programs_to_Madagascar)

#### RESUMO DAS OPÇÕES

[\-h] [\-\-help] [-v] [\-\-version] [\-c]

#### DESCRIÇÃO DAS OPÇÕES

\-h, \-\-help
Exibe a mensagem de ajuda do programa e sai.

\-v, \-\-version
Exibe a versão do programa e sai.

\-c <diretorio>
Compila e instala os programas em <diretorio> na cópia
local do pacote MADAGASCAR.

#### EXEMPLOS DE USO

* Compilar e instalar os programas de $RSFSRC/user/<diretorio> na instalação
do MADAGASCAR.

```sh
~$ comp -c <diretorio>
```

[Para mais detalhes consulte os manuais de uso dos programas desta biblioteca](https://github.com/Dirack/Shellinclude/blob/master/manuais).