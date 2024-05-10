# Guia de Inicialização do Git

O Git é uma ferramenta essencial para o controle de versão de código-fonte e colaboração em projetos de desenvolvimento de software. Este guia foi elaborado para auxiliar no aprendizado e uso básico do Git, desde a instalação até o fluxo de trabalho básico e comandos úteis.

Se você é novo no Git ou deseja relembrar conceitos e comandos fundamentais, este guia é para você. Vamos abordar desde a configuração inicial do Git até tarefas avançadas, como ramificação e fusão de branches.

Sinta-se à vontade para explorar e experimentar os comandos apresentados neste guia. O Git é uma ferramenta poderosa que pode melhorar significativamente a eficiência do seu trabalho em equipe e o controle sobre o código-fonte dos seus projetos.

Vamos começar!

## Configuração Inicial

1. **Instalação**: Faça o download e instale o Git a partir do [site oficial do Git](https://git-scm.com/).

2. **Configuração do Usuário**: Configure seu nome de usuário e endereço de e-mail globalmente com os seguintes comandos:
```sh
   git config --global user.name "Seu Nome"
   git config --global user.email "seu-email@example.com"
```
3. **Verificação de Configuração:** Verifique suas configurações com
```sh
    git config --global --list
```

## Configuração Inicial

1. **Clonagem de um Repositório Existente**: Para clonar um repositório existente para sua máquina local, use:
```sh
   git clone <url-do-repositorio>
```

2. **Inicialização de um Novo Repositório**: Para iniciar um novo repositório em um diretório existente, use:
```sh
   git init
```

## Fluxo de Trabalho Básico

1. **Adicionar Alterações**: Adicione arquivos modificados ao índice para prepará-los para o commit:
```sh
    git add .  -para todos os arquivos da pasta
    git add <arquivo1> <arquivo2> ...
```

2. **Commit de Alterações**: Confirme as alterações adicionadas ao índice:
```sh
   git commit -m "Mensagem do Commit"
```

3. **Envio de Alterações**: Envie suas alterações para o repositório remoto:
```sh
   git pull origin <branch>
```

## Ramificação e Fusão

1. **Criação de uma Nova Branch:** Crie uma nova branch para trabalhar em uma nova funcionalidade:
```sh
    git checkout -b <nome-da-branch>
```

2. **Mudança entre Branches:** Crie Mude entre branches existentes:
```sh
    git checkout <nome-da-branch>
```

3. **Fusão de Branches:** Funda uma branch específica com a branch atual:
```sh
    git merge <nome-da-branch>
```

4. **Remoção de Branches:** Remova uma branch específica:
```sh
    git branch -d <nome-da-branch>
```

## Extras

- **Ignorar Arquivos**: Use um arquivo `.gitignore` para especificar quais arquivos devem ser ignorados pelo Git.

- **Visualização de Histórico**: Visualize o histórico de commits:
```sh
   git log
```

- **Visualização de Diferenças**: Visualize as diferenças entre arquivos:
```sh
   git diff
```

## Outros Comandos Úteis

Aqui estão alguns outros comandos do Git que podem ser úteis para o seu trabalho diário:

- **`git status`**: Verifica o estado atual do repositório.
- **`git remote`**: Lista os repositórios remotos configurados.
- **`git fetch`**: Busca as alterações do repositório remoto, mas não as mescla no branch atual.
- **`git reset`**: Desfaz alterações locais específicas e redefine o estado do repositório.
- **`git checkout -- <arquivo>`**: Descarta as alterações feitas em um arquivo específico.
- **`git remote add <nome> <url>`**: Adiciona um novo repositório remoto.
- **`git remote remove <nome>`**: Remove um repositório remoto.
- **`git tag <nome>`**: Cria uma tag para marcar pontos importantes na história do repositório.
- **`git show <tag>`**: Exibe informações sobre uma tag específica.
- **`git tag -d <tag>`**: Remove uma tag específica.
- **`git push --tags`**: Envia todas as tags locais para o repositório remoto.

Lembre-se de consultar a documentação oficial do Git para mais informações sobre esses e outros comandos.

## Mensagem Final

Parabéns! Você concluiu o guia básico de inicialização do Git. Esperamos que este documento tenha sido útil para você começar a utilizar o Git em seus projetos de desenvolvimento.


