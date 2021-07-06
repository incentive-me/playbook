Neste arquivo se encontram algumas instruções para configurar o desenvolvimento integrado com docker pelo VS Code.

Para começar, abra o link abaixo e siga os passos.

[Visual Studio Code Remote - Containers](https://code.visualstudio.com/docs/remote/containers)

Caso tenha algum problema, temos algumas soluções para os SO's:

# Windows:

## 1. Instalação distribuição Ubuntu (WSL):

- Clique [aqui](https://aka.ms/wslstore), voce será redirecionado para a microsoft Store.

- Escolha e instale a distribuição Ubuntu.

- Crie um usuario e senha.

## 2. Instalação Docker Desktop:

- Clique [aqui](https://www.docker.com/products/docker-desktop) para instalação do Docker.

- Após a instalação, abra o Docker desktop e clique sobre o icone de engrenagem no canto
  superior direito.
- Encontre a opção Resources > WSL INTEGRATION

- Em "Enable integration with additional distros:" Habilite a opção Ubuntu.

## 3.Instalações de extenções para o VsCode:

- [Remote-WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)

- [Remote-Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

- [docker vs Code](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)

## 4. Após o Clone do Repositório do projeto:

- Abra uma nova janela do VSCode.

- Siga o passo da Imagem abaixo e click sobre "Open Folder in WSL" ![Step 1](./imgs/step1.png)

- Siga o passo da Imagem abaixo e click sobre "Reopen in Container" ![Step 2](./imgs/step2.png)

- Siga o passo da Imagem abaixo e click sobre "Rebuild Container" ![Step 3](./imgs/step3.png)

## 5 - Conflito Com Git:

- Caso git apresente modificações irregulares, com o terminal na pasta do repositorio execute o comando: `git config --global core.autocrlf true`

# Linux

Problema com autorização para escrita.
Execute

```bash
sudo chown -R <seu_user> diretório/para/o/projeto
```