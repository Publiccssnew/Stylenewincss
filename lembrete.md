### Armazenar lembretes e idéias do usuário.

LEMBRETE é um auxiliar para a memória, ideal para armazenar idéias, números de telefone e pequenas listas de tarefas.

#### RESUMO DAS OPÇÕES
[\-h] [\-\-help] [-v] [\-\-version] [\-a] [\-\-add]
[\-l] [\-\-list] [\-r] [\-\-remove] 

#### DESCRIÇÃO DAS OPÇÕES

\-h, \-\-help
Exibe a mensagem de ajuda do programa e sai.

\-v, \-\-version
Exibe a versão do programa e sai.

\-a, \-\-add
Adicionar novo lembrete.

\-l, \-\-list
Listar todos os lembretes ou um lembrete específico.

\-r, \-\-remove
Remover lembrete.

#### EXEMPLOS DE USO

* Adicionar um lembrete <tag> com a mensagem <Mensagem>.

```sh
~$ lembrete -a tag -m "Mensagem"
```

* Listar um lembrete específico.

```sh
~$ lembrete -l tag
```

* Listar todos os lembretes.

```sh
~$ lembrete -l
```

* Remover lembrete.

```sh
~$ lembrete -r tag
```

[Para mais detalhes consulte os manuais de uso dos programas desta biblioteca](https://github.com/Dirack/Shellinclude/blob/master/manuais).