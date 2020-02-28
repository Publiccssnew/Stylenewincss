#### Formatar mensagem de ajuda dos programas da biblioteca Shellinclude

#### Descrição das funções 

# Fornecer os parâmetros para a função 'exibirMensagemAjudaProgramaFormatada'
# da seguinte maneira:
#
#               $1 NOME DO PROGRAMA
#               $2 DESCRIÇÃO
#               $3 PARÂMETROS
#               $4 EXEMPLO DE USO
#
# Os parâmetros devem ser passados em uma variável em que cada linha é um parâmetro,
# separado de sua legenda explicativa por '::' como no exemplo abaixo:
#
# PARÂMETROS="-h --help:: Exibe esta mensagem de ajuda e sai
#             -v --version:: Exibe a versão do programa e sai
#             -c:: Realiza alguma coisa"
#
# Exemplo de uso desta biblioteca:
#
#       ~$ source mensagemAjuda.sh
#       ~$ NOME_PROGRAMA="TESTE"
#       ~$ DESCRICAO="Este é um teste"
#       ~$ PARAMETROS="-h --help::Exibe ajuda e sai"
#       ~$ EXEMPLO_DE_USO="Exemplo de teste"
#       ~$ exibirMensagemAjudaProgramaFormatada "$NOME_PROGRAMA" "$DESCRICAO" "$PARAMETROS" "$EXEMPLO_DE_USO"
#
#       Saída esperada:
#
#               NOME
#                       TESTE
#               DESCRIÇÃO
#                       Este é um teste
#               PARÂMETROS
#                       -h --help Exibe ajuda e sai
#               EXEMPLO DE USO
#                       Exemplo de teste

formatarTabelaParametros(){


        TABELA_PARAMETROS_FORMATADA=$(echo "$1" | sed 's/^/\\t\\033[00;01m/' | sed 's/::/ \\033[m/' )

        echo "$TABELA_PARAMETROS_FORMATADA"

}
