# BasicoGit

Este documento apresenta os passos básicos para iniciar um projeto com Git e enviar as alterações para o GitHub.

## Criar pasta
Primeiro, crie uma pasta para o projeto.

![criar pasta](CriarPasta.png)

## Acessar a pasta
Entre na pasta criada.

![ir para a pasta](IrPasta.png)

## Iniciar o Git
No terminal, inicialize o Git dentro da pasta.

![Iniciar git](IniciarGit.png)

Depois disso, o Git estará pronto para acompanhar as alterações do projeto.

![Git iniciado](GitIniciado.png)

## Criar repositório no GitHub
Acesse o GitHub e crie um novo repositório para o projeto.

![Criar repositório](CriarRepositorio.png)

Essa é a tela inicial quando cria-se um repositório

![Tela Inicial](telaRepoInicial.png)

## Conectar o repositório local ao remoto
No terminal, adicione o repositório remoto ao projeto local utilizando o seguinte comando:

```bash
git remote add origin <link-do-repositorio>
```

![Adicionar origem remota](addOrigemRemota.png)

## Criar o README
Crie o arquivo README.md com as informações do projeto.

![Criar README](CriarReadme.png)

## Adicionar alteração

Adicione essa alteração com o comando
```bash
git add <nome-do-arquivo>
```
também pode ser feito utilizando o (por isso as duas barras "||" na imagem): 
```bash
git add .
```
esse comando adiciona todos os arquivos, sendo ideal para se utilizar quando eles mudam as mesmas coisas.

![Adicionar README](addArquivo.png)

## Fazer commit
Crie um commit para salvar as alterações no histórico do Git com o comando:

```bash
git commit -m "Adiciona README"
```

![Commit do arquivo](commitArquivo.png)

![Arquivo commitado](ArquivoCommitado.png)

## Trabalhar com branches
Após commitar, envia-se as alterações para o repositório remoto, mas antes deve-se verificar a branch atual, fazendo:

```bash
git branch
```

![Verificar branch](verificarBranch.png)

![Branch verificada](branchVerificada.png)

Se quiser criar uma nova branch:

```bash
git checkout -b nome-da-branch
```

## Enviar para o GitHub
Assim, quando verificado se está na branch certa, as alterações podem ser enviadas para o repositório remoto com o seguinte comando:

```bash
git push origin main
```

![Push main](pushMain.png)

![Modificações enviadas](modEnviadas.png)

Assim fica a tela do github com as mudanças feitas:

![Tela com as mudanças](telaRepoReadme.png)

## Fazer alterações e enviar novamente
Depois de editar arquivos, adicione, faça commit e envie as mudanças.


Abrir a pasta do projeto e editar o arquivo README.md:

![Editar README](abrirDir.png)

![tela do readme no code](telaCodeReadme.png)

No code, modificamos o arquivo README.md:

![Modificar README](modReadme.png)

Então, adicionamos a modificação:

![Adicionar modificação](addModReadme.png)

Depois, fazemos o commit da modificação:

![Commit da modificação](commitModReadme.png)

![Modificar README commitada](modReadmeCommitada.png)

Com isso, enviamos a modificação para o repositório remoto:
![Push da modificação](pushModReadme.png)

![Modificar README enviada](modReadmeEnviada.png)

Assim fica a tela do GitHub com a modificação feita:

![Tela com a modificação](telaNovoReadme.png)

Esses passos formam o fluxo básico do Git: criar projeto, iniciar o Git, adicionar arquivos, fazer commit e enviar para o GitHub.