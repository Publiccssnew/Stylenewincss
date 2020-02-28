### Formatar mensagem de erro dos programas da biblioteca Shellinclude

#### Descrição das funções 

A função _exibirMensagemErroProgramaFormatada_ recebe os parâmetros da seguinte maneira:

- $1 NOME_PROGRAMA
- $2 NUMERO_ERRO
- $3 MENSAGEM_ERRO

Exibe o erro na tela com o seguinte comando echo e encerra a execução com exit: 

```sh
echo -e "\033[31m$NOME_PROGRAMA: ERRO($NUMERO_ERRO):  $MENSAGEM_ERRO\033[m"

exit "$NUMERO_ERRO"
```

Para compreender melhor a utilização desta biblioteca, utilize o seguinte exemplo de uso no terminal do shell:

```sh
~$ source mensagemAjuda.sh
~$ NOME_PROGRAMA="TESTE"
~$ DESCRICAO="Este é um teste"
~$ PARAMETROS="-h --help::Exibe ajuda e sai"
~$ EXEMPLO_DE_USO="Exemplo de teste"
~$ exibirMensagemAjudaProgramaFormatada "$NOME_PROGRAMA" "$DESCRICAO" "$PARAMETROS" "$EXEMPLO_DE_USO"

              NOME
                      TESTE
              DESCRIÇÃO
                      Este é um teste
              PARÂMETROS
                      -h --help Exibe ajuda e sai
              EXEMPLO DE USO
                      Exemplo de teste
```