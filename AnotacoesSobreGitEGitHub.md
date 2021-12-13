# Git e GitHub

### Salvar versões diferentes de um projeto em disco 
Visa possibilitar o acesso de uma versão anterior desejada. O problema é o espaço ocupado em um disco rígido e a falta de organização compromete a segurança dos dados.

### Controle de versão
Automatiza o gerenciamento de versões de um projeto.

### Software de controle de versão(VCS) centralizado
O usuário sempre está conectado ao servidor que faz o controle de versão.

### VCS distribuído
A versão do projeto não é gerida por um servidor conectado diretamente ao usuário e sim por um software instalado localmente. 

### Git
É um software de controle de versão. É um repositório local.

### GitHub
Plataforma de rede social para programadores. É um repositório remoto.

### Repositório
É uma pasta onde o projeto é hospedado e divulgado.

### Commit
Ação de enviar diretórios/arquivos monitorado para um repositório central.

### Estágios dos arquivos no git

![Ciclo de vida em um VCS ](./cicloArquivosGit.png)

- **Untracked:** O projeto não foi visto pelo git
- **Unmodified:** O projeto está no repositório em estado de espera para ser alterado.
- **Modified:** Quando o projeto é alterado é permitido adicioná-lo ao estado de Staged através do comando git add.
- **Staged:** Quando o projeto é alterado é permitido adicioná-lo ao repositório central.

## Comandos

`git init`: Cria um diretório chamado .git que possui arquivos responsáveis por gerenciar versões de um projeto no diretório atual, ou seja, cria um repositório central.

`git status`: Mostra o status atual do repositório.

`git add nomeDoArquivo`: Adiciona ou modifica o arquivo o preparando para ser comitado.

`git commit -am “mensagem descritiva”`: Cria uma versão do projeto adicionando os diretórios/arquivos ao repositório central. O parâmetro -m permite adicionar uma mensagem descrevendo a versão do projeto, o que sempre é recomendado por boas práticas.

`git log`: Mostra as informações registradas de quando um commit foi feito.

`git show idDoCommit`: Mostra os detalhes de um commit específico. O id de um commit específico, pode ser consultado através do comando `git log`.

`git checkout nomeDoArquivo`: Retorna o arquivo para o estado unmodified.

`git reset --soft idDoCommit`: Retorna um projeto commitado para o estado anterior ao Staged.

`git reset --mixed idDoCommit`: Retorna um projeto commitado para o estado anterior ao Modified.

`git reset --hard idDoCommit`: Apaga um commit realizado.






