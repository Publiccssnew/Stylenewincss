### Formatar mensagem de ajuda dos programas da biblioteca Shellinclude

#### Descrição das funções 

A função _exibirMensagemAjudaProgramaFormatada_ recebe os parâmetros da seguinte maneira:

- $1 NOME DO PROGRAMA
- $2 DESCRIÇÃO
- $3 PARÂMETROS
- $4 EXEMPLO DE USO

Os parâmetros devem ser passados dentro de uma variável em que cada linha é um parâmetro,
separados de sua legenda explicativa por '::' como no exemplo abaixo:

```sh
PARÂMETROS="-h --help:: Exibe esta mensagem de ajuda e sai
            -v --version:: Exibe a versão do programa e sai
            -c:: Realiza alguma coisa"
```

A função _formatarTabelaParametros_ recebe a variável com os parâmetros no formato descrito acima, adiciona a tabulação no início da linha e substitui o caractere separador '::' por um espaço em branco.

Para compreender melhor a utilização desta biblioteca, utilize o seguinte exemplo de uso em um arquivo 'script.sh':

```sh
#!/bin/bash
source mensagemAjuda

NOME_PROGRAMA="TESTE"
DESCRICAO="Este é um teste"
PARAMETROS="-h --help::Exibe ajuda e sai"
EXEMPLO_DE_USO="Exemplo de teste"

exibirMensagemAjudaProgramaFormatada "$NOME_PROGRAMA" "$DESCRICAO" "$PARAMETROS" "$EXEMPLO_DE_USO"
```

A saída esperada será:

```sh
~$ ./script.sh

              NOME
                      TESTE
              DESCRIÇÃO
                      Este é um teste
              PARÂMETROS
                      -h --help Exibe ajuda e sai
              EXEMPLO DE USO
                      Exemplo de teste
```