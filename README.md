# BasicoGit

Este documento apresenta os passos básicos para iniciar um projeto com Git e enviar as alterações para o GitHub.

## 1. Criar pasta
Primeiro, crie uma pasta para o projeto.

![criar pasta](CriarPasta.png)

## 2. Acessar a pasta
Entre na pasta criada.

![ir para a pasta](IrPasta.png)

## 3. Iniciar o Git
No terminal, inicialize o Git dentro da pasta.

![Iniciar git](IniciarGit.png)

Depois disso, o Git estará pronto para acompanhar as alterações do projeto.

![Git iniciado](GitIniciado.png)

## 4. Criar repositório no GitHub
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

## 6. Criar o README
Crie o arquivo README.md com as informações do projeto.

![Criar README](CriarReadme.png)

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

## 8. Fazer commit
Crie um commit para salvar as alterações no histórico do Git com o comando:

```bash
git commit -m "Adiciona README"
```

![Commit do arquivo](commitArquivo.png)

![Arquivo commitado](ArquivoCommitado.png)

## 9. Enviar para o GitHub
Enviando as alterações para o repositório remoto.

```bash
git push -u origin main
```

![Push main](pushMain.png)

![Modificações enviadas](modEnviadas.png)

## 10. Trabalhar com branches
Para verificar a branch atual, use:

```bash
git branch
```

![Verificar branch](verificarBranch.png)

![Branch verificada](branchVerificada.png)

Se quiser criar uma nova branch:

```bash
git checkout -b nome-da-branch
```

## 11. Fazer alterações e enviar novamente
Depois de editar arquivos, adicione, faça commit e envie as mudanças.

![Modificar README](modReadme.png)

![Commit da modificação](commitModReadme.png)

![Modificar README commitada](modReadmeCommitada.png)

![Modificar README enviada](modReadmeEnviada.png)

![Push da modificação](pushModReadme.png)

Esses passos formam o fluxo básico do Git: criar projeto, iniciar o Git, adicionar arquivos, fazer commit e enviar para o GitHub.