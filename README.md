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

