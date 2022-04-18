## Como contribuir com este projeto?

A seguir a descrição detalhada do passo-a-passo para contribuir com este projeto:

**1. Crie uma issue para a sua modificação**

A forma mais fácil de contribuir com este projeto é através de sugestões de modificações nas issues. 
Na aba issues você terá a opção de 4 templates de modificações: Feature request (Para solicitar uma nova funcionalidade), Documentation (Para solicitar documentação em arquivos README, exemplos de uso, wikis e outros), Bug report (Para reportar bugs) e Test requests (Para solicitar testes automatizados de alguma funcionalidade).

Escolha um template e preencha a descrição da sua solicitação. Não é necessário apagar os títulos em negrito dos templates de issues. Seja o mais claro possível, e aproveite para descrever bem a sua solicitação, utilize imagens e trechos de código se for preciso.

Se a sua contribuição é a solução de uma issue que já está definida, ignore este passo.

**2. Faça o _fork_ do projeto em <https://github.com/Dirack/Shellinclude/fork>**

Se você quiser contribuir incorporando as suas próprias alterações a este projeto, faça um fork para a sua conta no github e leia a Licença de uso.

Este projeto é de código aberto e distribuído sob a lincença GPL3. Ao fazer o fork você automaticamente
concorda com os termos dispostos nesta Licença de uso.

**3. Crie uma _branch_ para sua modificação.**

No seu fork do projeto, crie uma nova branch com um nome que faça referência à issue que voce criou no passo 1 da seguinte maneira (ID é o número da issue): 

- Se a issue que você criou é uma _Feature request_, o nome da branch será 'feature/issue/ID' 
- Se a issue que você criou é uma _Documentation request_, o nome da branch será 'documentation/issue/ID' 
- Se a issue que você criou é uma _Test request_, o nome da branch será 'test/issue/ID' 
- Se a issue que você criou é uma _Bug report_, o nome da branch será 'hotfix/issue/ID'

As branches principal e de desenvolvimento também seguem regras de nomeação:

- A branch de desenvolvimento é aberta pelo administrador do repositório, seu nome é 'develop/VERSAO' (Versão é a tag da versão atual que está sendo desenvolvida)
- A branch principal é a master e somente o administrador pode fazer modificações nesta branch

A incorporação das branches ao repositório seguem a regra do _gitflow_:

- As branches a seguir são abertas e incorporadas nas branches de desenvolvimento da versão atual: Branches features, documentation e test.

- As branches a seguir são abertas e incorporadas na master: Branches develop e hotfix.

- A branch master só recebe modificações de novas versões do repositório provenientes de develop e correções de bug de hotfix

- A branch develop recebe modificações provenientes de qualquer branch, incluindo as correções de bugs da master

**3. Faça o _commit_ com uma mensagem clara (título de no máximo 50 caracteres e dois parágrafos de texto).**

O histórico de commits é tão importante para este repositório quanto o conteúdo de suas modificações. O padrão
Aqui utilizado é de mensagens de commit com o título de no máximo 50 caracteres e um a dois parágrafos descrevendo cada modificação. 

_Pull Requests_ com histórico de commits insuficiente serão rejeitados.
Faça referências a outros commits se for necessário, a referência a issue que está sendo solucionada é obrigatória e é feita acrescentando #ID (ID da issue) na mensagem ou título do commit. 

Se a modificação for muito pequena (como o valor de uma variável, ou uma linha de código) o commit poderá ter
apenas o título da mensagem de commit. Porém, para modificações mais significativas os commits devem ter
título e mensagens como descrito nos parágrafos anteriores.

Evite comentar o código para explicar a lógica de suas modificações, isto pode ser feito
nas mensagens de commit mais extensivamente. Se a sua explicação for muito longa (mais de dois parágrafos),
é melhor dividir as alterações em mais commits com mensagens mais claras e curtas.

Utilize nomes de variáveis e funções claros e com contexto, de preferência camelCase para funções
e caixa alta para nomes de variáveis.
Exemplo, 'ARQUIVO_TEMP' é melhor que 'TMP', ou 'NOME_USUARIO' é melhor que 'NOME'.
E 'formataNomeDiretorio' é melhor que 'fmtdir'.

A seguir um exemplo de commit padronizado que se refere à issue 3:

```
Programa morse - enviar email pelo terminal #3

Morse utiliza o sendemail para enviar emails através do terminal. Sua
interface é baseada em Dialog, um programa que gera caixas de diálogo
interativas na tela do terminal.
```

Outra prática importante é adicionar cabeçalhos aos seus códigos fonte, seguindo o template
abaixo:

```sh
#!/bin/bash
#
# nomeDoPrograma (Shell Script)
#
# Dependências: -lynx. Utilize 'sudo apt-get install lynx' para instalar.
#
# Objetivo: Baixar arquivos SConstruct da página do MADAGASCAR para a pasta atual
# no formato correto do SConstruct.
# 
# Site: http://www.dirackslouge.online
#
# Versão 1.0
#
# Programador: Rodolfo A. C. Neves 30/06/2019
# 
# Email (Manutenção): rodolfo_profissional@hotmail.com
# 
# Licença: GPL-3.0 <https://www.gnu.org/licenses/gpl-3.0.txt>.
```

**4. Faça o _Push_ das suas modificações no seu repositório.**

Basta utilizar o comando a seguir para fazer o push das suas alterações já commitadas para a branch correspondente no seu fork  do repositório:

```sh
~$ git push origin feature/issue/3
```

Depois de fazer o push para o seu fork do repositório, faça o pull request para a branch correspondente deste repositório, seguindo a regra descrita no passo 3.

**5. Crie um novo _Pull Request_ com uma descrição clara de suas modificações.**

O seu Pull Request deve ter uma descrição mais detalhada das modificações e do propósito delas,
utilize imagens e trechos de código para detalhar a sua contribuição sempre que possível.

Acrescentar exemplos de uso e testes automatizados ao seu Pull Request aumenta a probabilidade de aceitação.
Não esqueça de documentar estes testes e exemplos em arquivos README e agrupá-los em um diretório
separado.

Se forem testes automatizados, descreva o resultado esperado, o teste e o critério utilizado para a validação.