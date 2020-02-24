getscons - Baixar e formatar arquivo SConstruct do site oficial do Madagascar.
Listar todos os papers da aba 'Reproducible Documents' e seus respectivos SConstruct's.

.SH RESUMO
.B getscons
[\-h] [\-\-help] [-v] [\-\-version] [\-l] [\-u] [\-\-update] [\-s]

.SH DESCRIÇÃO
.PP
GETSCONS é um auxiliar de pesquisa de papers no site oficial do MADAGASCAR
buscando um determinado assunto nas descrições disponíveis no site.
Ao utilizar este programa você pode baixar diretamente um SConstruct já formatado,
através do terminal, fornecendo ao programa um link de uma página do site do MADAGASCAR 
que contenha algum SConstruct.

.SH OPÇÕES
GETSCONS aceita as seguintes opções:
.TP 8
.B  \-h, \-\-help
Exibe a mensagem de ajuda do programa e sai.
.TP 8
.B \-v, \-\-version
Exibe a versão do programa.
.TP 8
.B \-l <link>
Baixa o SConstruct da página <link> para a pasta atual.
Este SConstruct já terá o nome e formato padrão de Script
do MADAGASCAR.
.TP 8
.B \-u, \-\-update
Atualiza a lista de papers do Madagascar na sua máquina.
.TP 8
.B \-s <subject>
Pesquisa na lista de papers disponível no site por um determinado
assunto <subject>.

.SH EXEMPLOS DE USO
.PP
Baixar o SConstruct da página <link> para a pasta atual.

	~$ getscons -l <link>
.PP
Atualizar a listagem dos links dos papers para o programa getscons.

	~$ getscons --update

.PP
Pesquisar papers sobre o assunto 'diffraction'.

	~$ getscons -s 'diffraction'

[Para mais detalhes consulte os manuais de uso dos programas desta biblioteca](https://github.com/Dirack/Shellinclude/blob/master/manuais).