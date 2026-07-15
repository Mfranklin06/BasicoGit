# BasicoGit

Este documento apresenta os passos básicos para iniciar um projeto com Git e enviar as alterações para o GitHub.

## Criar pasta
Primeiro, crie uma pasta para o projeto.

![criar pasta](public/CriarPasta.png)

## Acessar a pasta
Entre na pasta criada.

![ir para a pasta](public/IrPasta.png)

## Iniciar o Git
No terminal, inicialize o Git dentro da pasta.

![Iniciar git](public/IniciarGit.png)

Depois disso, o Git estará pronto para acompanhar as alterações do projeto.

![Git iniciado](public/GitIniciado.png)

## Criar repositório no GitHub
Acesse o GitHub e crie um novo repositório para o projeto.

![Criar repositório](public/CriarRepositorio.png)

Essa é a tela inicial quando cria-se um repositório

![Tela Inicial](public/telaRepoInicial.png)

## Conectar o repositório local ao remoto
No terminal, adicione o repositório remoto ao projeto local utilizando o seguinte comando:

```bash
git remote add origin <link-do-repositorio>
```

![Adicionar origem remota](public/addOrigemRemota.png)

## Criar o README
Crie o arquivo README.md com as informações do projeto.

![Criar README](public/CriarReadme.png)

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

![Adicionar README](public/addArquivo.png)

## Fazer commit
Crie um commit para salvar as alterações no histórico do Git com o comando:

```bash
git commit -m "Adiciona README"
```

![Commit do arquivo](public/commitArquivo.png)

![Arquivo commitado](public/ArquivoCommitado.png)

## Trabalhar com branches
Após commitar, envia-se as alterações para o repositório remoto, mas antes deve-se verificar a branch atual, fazendo:

```bash
git branch
```

![Verificar branch](public/verificarBranch.png)

![Branch verificada](public/branchVerificada.png)

Se quiser criar uma nova branch:

```bash
git checkout -b nome-da-branch
```

## Enviar para o GitHub
Assim, quando verificado se está na branch certa, as alterações podem ser enviadas para o repositório remoto com o seguinte comando:

```bash
git push origin main
```

![Push main](public/pushMain.png)

![Modificações enviadas](public/modEnviadas.png)

Assim fica a tela do github com as mudanças feitas:

![Tela com as mudanças](public/telaRepoReadme.png)

## Fazer alterações e enviar novamente
Depois de editar arquivos, adicione, faça commit e envie as mudanças.


Abrir a pasta do projeto e editar o arquivo README.md:

![Editar README](public/abrirDir.png)

![tela do readme no code](public/telaCodeReadme.png)

No code, modificamos o arquivo README.md:

![Modificar README](public/modReadme.png)

Então, adicionamos a modificação:

![Adicionar modificação](public/addModReadme.png)

Depois, fazemos o commit da modificação:

![Commit da modificação](public/commitModReadme.png)

![Modificar README commitada](public/modReadmeCommitada.png)

Com isso, enviamos a modificação para o repositório remoto:
![Push da modificação](public/pushModReadme.png)

![Modificar README enviada](public/modReadmeEnviada.png)

Assim fica a tela do GitHub com a modificação feita:

![Tela com a modificação](public/telaNovoReadme.png)

Esses passos formam o fluxo básico do Git: criar projeto, iniciar o Git, adicionar arquivos, fazer commit e enviar para o GitHub.