* v1.1 (Estável)
    * Primeira versão estável (Em desenvolvimento).
    * Permite ao programa comp localizar os diretórios do Madagascar na cópia local a partir da variável de ambiente $RSFSRC (referenciado na [issue#19](https://github.com/Dirack/Shellinclude/issues/19)).
    * Remove as opções obsoletas do programa getscons (referenciado na [issue#20](https://github.com/Dirack/Shellinclude/issues/20))
    * Todos os programas agora utilizam mensagens padronizadas de erro e de ajuda (referenciado na [issue#24](https://github.com/Dirack/Shellinclude/issues/24) e [issue#30](https://github.com/Dirack/Shellinclude/issues/30))
    * Corrige o bug no programa img, ao rodar a opção -i em uma pasta sem arquivos '.vpl' mas com subdiretórios que contém arquivos '.vpl' (referenciado na [issue#31](https://github.com/Dirack/Shellinclude/issues/31))
    * Corrige o número de versão de todos os programas para 1.1 (referenciado na [issue#32](https://github.com/Dirack/Shellinclude/issues/32))

* [v1.0](https://github.com/Dirack/Shellinclude/releases/tag/v1.0-beta.1) (Beta)
    * Versão Beta dos principais scripts:
        * **backup**: Fazer o backup de um arquivo ou de uma lista de arquivos em um arquivo zipado na pasta atual.
        * **cabecalho**: Gerar o cabeçalho para um arquivo de programa com objetivo, nome do programa e etc.
        * **comp**: Compilar e instalar programas à versão local do pacote de processamento sísmico MADAGASCAR.
        * **getscons**: Baixar arquivos SConstruct da página do MADAGASCAR para a pasta atual.
        * **img**: Converter arquivos .vpl (arquivos de imagem do MADAGASCAR) em imagens .jpeg
        * **jonas**: Criar atalhos para pastas e aliases permanentes.
        * **lembrete**: Armazenar lembretes e idéias.
        * **morse**: Enviar email pelo terminal.