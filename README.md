# Summary-About-Git-GitHub
Summary About Git GitHub In README

# DIO | Resumos Git e GitHub

Repositório para armazenar resumos sobre Git e GitHub
do curso Versionamento de Código com Git e GitHub da
[DIO Cursos](https://www.dio.me/).

## 📕 Documentação
- [Documentação Git](https://git-scm.com/doc).
- [Documentação GitHub](https://docs.github.com/).

## 💻 Comandos Git


#### Configurando o Git:
- Nome de usuário:
  ``` git config --global user.name "Seu Nome" ```
- Endereço de e-mail:
  ``` git config --global user.email "seuemail@example.com" ```
  
##### A opção init.defaultBranch no git config é utilizada para definir a branch padrão que será criada quando um novo repositório Git for inicializado utilizando o comando git init.
``` git config --global init.defaultBranch main ```
##### Ver Branch Padrão:
``` git config init.defaultBranch ```

### Criando e Clonando Repositórios:
### Criando um Novo Repositório Local:

1 - Inicialize Um Novo Repositório:
- Navegue até o diretório do seu projeto usando o terminal ou Git Bash e execute o seguinte comando para iniciar um novo repositório Git:
  ``` git init ```
  
2 - Adicione Seus Arquivos Ao Repositório:
- Adicione os arquivos do seu projeto ao repositório Git usando git add:
  ``` git add . ```

3 - Confirme suas alterações:
- Confirme as alterações com git commit:
  ``` git commit -m "Primeiro commit" ```

4 - Envie suas alterações para o repositório remoto:
  ``` git push -u origin <Enviar Branch>" ```
  
5 - Atualize seu repositório local:
  ``` git pull origin <Enviar Branch>" ```

### Clonando um Repositório Existente:

1 - Clone o repositório:
- Use o comando git clone seguido pelo URL do repositório que você deseja clonar:
  ``` git clone <url_do_repositorio> ```
- Substitua <url_do_repositorio> pelo URL do repositório que você deseja clonar. Por exemplo:
  ``` git clone https://github.com/usuario/nome-do-repositorio.git ```

### Desfazendo Alterações no Repositório Local:  

1 - Este comando restaura o arquivo README.md para o estado em que estava na última confirmação. Se você fez alterações no arquivo e ainda não as adicionou ao stage, git restore desfará essas alterações. Se você já adicionou as alterações ao stage, elas permanecerão no stage, mas o arquivo README.md será restaurado para o estado da última confirmação:
``` git restore README.md ```
  
2 - Este comando remove recursivamente (-r) e forçadamente (-f) o diretório .git e todos os seus subdiretórios e arquivos. O diretório .git é o diretório que contém todos os metadados e informações de controle de versão do seu repositório Git. Removê-lo é uma ação drástica e efetivamente desfaz a rastreabilidade e a história do seu repositório Git. Use este comando com extrema cautela, pois ele não pode ser desfeito facilmente e resultará na perda irreversível de todos os registros de commit, branches, tags e configurações específicas do Git no seu projeto:
``` rm -rf .git ```

### Trabalhando com Branches:

1 - Criar uma nova branch:
- Isso cria uma nova branch com o nome especificado, mas não muda para ela:
``` git branch <nome_da_branch> ```
  
2 - Criar uma nova branch e mudar para ela:
- Isso cria uma nova branch com o nome especificado e muda imediatamente para ela:
``` git checkout -b <nome_da_branch> ```

3 - Listar todas as branches no repositório:
- Isso lista todas as branches no repositório e marca com um asterisco (*) a branch atual:
``` git branch ```

4 - Mudar para outra branch:
- Isso muda para a branch especificada:
``` git checkout <nome_da_branch> ```

5 - Mesclar uma branch para a branch atual:
- Isso mescla as alterações da branch especificada para a branch atual:
``` git merge <nome_da_branch> ```

6 - Excluir uma branch localmente:
- Isso exclui a branch especificada localmente. Use -D em vez de -d se você quiser excluir a branch mesmo que haja alterações não mescladas:
``` git branch -d <nome_da_branch> ```

7 - Excluir uma branch remotamente:
- Isso exclui a branch especificada no repositório remoto:
``` git push origin --delete <nome_da_branch> ```

8 - Criar uma nova branch com base em outra branch existente, você pode usar o comando git checkout com a opção -b. Aqui está como fazer isso:
``` git checkout -b <nome_da_nova_branch> <nome_da_branch_base> ```

- Isso criará uma nova branch com o nome especificado <nome_da_nova_branch> e a baseará na branch especificada <nome_da_branch_base>. Por exemplo, se você deseja criar uma nova branch chamada nova-feature com base na branch develop, você usaria o seguinte comando:
``` git checkout -b nova-feature develop ```

- Isso criará uma nova branch chamada nova-feature com base na branch develop, e você será automaticamente mudado para a nova branch, pronto para começar a trabalhar nela.

  ### Convenções de Branch:

  #### Convenções de nomenclatura de branches são úteis para organizar e manter a consistência em um projeto Git, especialmente em equipes colaborativas. Aqui estão algumas convenções comuns de nomenclatura de branches:

1 - Master/Main Branch:
- Geralmente a branch principal do projeto.
- Nomes comuns incluem master ou main.
- Deve representar sempre a versão mais estável e de produção do código.

2 - Branches de Recursos/Features:
- Usadas para desenvolver novos recursos ou funcionalidades.
- Nomes geralmente descritivos do recurso que está sendo desenvolvido.
- Exemplos: feature/nova-autenticacao, feature/melhoria-interface.

3 - Branches de Correção de Bugs/Hotfixes:
- Usadas para corrigir bugs críticos na produção.
- Nomes geralmente descritivos do bug sendo corrigido.
- Exemplos: hotfix/conserto-login, hotfix/correcao-crash-app.

4 - Branches de Desenvolvimento:
- Usadas para integrar e testar novas funcionalidades antes de serem mescladas na branch principal.
- Nomes comuns incluem develop ou dev.
- Pode ser usada como base para branches de features.

5 - Branches de Liberação/Release:
- Usadas para preparar uma versão para lançamento.
- Geralmente mescladas de volta para a branch principal após o lançamento.
- Nomes geralmente descritivos do número da versão.
- Exemplos: release/1.0, release/2.0.

6 - Branches de Suporte/Support:
- Usadas para aplicar correções a versões antigas do software em produção.
- Nomes geralmente descritivos do número da versão.
- Exemplos: support/1.0, support/2.0.
  
### Este comando criará uma nova branch chamada feature/nova-funcionalidade com base na branch develop:
``` git checkout -b feature/nova-funcionalidade develop ```

  
