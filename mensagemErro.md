### Formatar mensagem de erro dos programas da biblioteca Shellinclude

#### Descrição das funções 

A função _exibirMensagemErroProgramaFormatada_ recebe os parâmetros da seguinte maneira:

- $1 NOME_PROGRAMA
- $2 NUMERO_ERRO
- $3 MENSAGEM_ERRO

Exibe o erro na tela com o seguinte comando _echo_ e encerra a execução com _exit_: 

```sh
echo -e "\033[31m$NOME_PROGRAMA: ERRO($NUMERO_ERRO):  $MENSAGEM_ERRO\033[m"

exit "$NUMERO_ERRO"
```

Para compreender melhor a utilização desta biblioteca, utilize o seguinte exemplo de uso dentro de um shell script chamado _script.sh_:

```sh
#!/bin/bash
# Arquivo script.sh

source mensagemErro

MENSAGEMERRO="Exemplo de uso da biblioteca mensagemErro"
exibirMensagemErroProgramaFormatada "$(basename $0)" "1" "$MENSAGEMERRO"
```

A saída esperada será:

```sh
~$ ./script.sh
script.sh: ERRO(1):  Exemplo de uso da biblioteca mensagemErro.sh
```