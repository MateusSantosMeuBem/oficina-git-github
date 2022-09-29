# Introdução a Git e GitHub

## História do Git
 - Como surgiu?
 - Para que serve?

## História do GitHub
 - Como surgiu?
 - Para que serve?

### Criando uma conta no GitHub
Para ser direcionado à página do GitHub [clique aqui](https://github.com/)!

### Baixar e configurar o Git
Para baixar o Git basta acessar o [link](https://git-scm.com/). Selecionar o download para Windows, baixar o instalador (32-bits ou 64-bits) e clicar para instalar.

#### Configurar as credenciais
 - Nome e email
```bash
git config --global user.name "<seu nome>"
```
```bash
git config --global user.email "<seu email do GitHub>"
```
 - Chave SSH
 ```bash
ssh-keygen -t rsa -C "<seu email do GitHub>"
 ```
- Verificar autenticação
```bash
ssh -T git@github.com
```

### Criando um repositório local
Na pasta do seu projeto rode no Git Bash o seguinte comando
```bash
git init
```
### Adionar arquivos à área de `stage`.
Arquivos selecionados
```bash
git add "<arquivo 1>" "<arquivo 2>"
```
Todos os arquivos
```bash
git add .
```

### "Commitar" os arquivos
```bash
git commit -m "<mensagem do commit>"
```
### Enviar repositório local para a nuvem
Conectar repositório local com o da nuvem
```bash
git remote add origin <endereço do repositório na nuvem>
```
Mudar-se para a branch Main (se necessário)
```bash
git branch -M main
```
Enviar repositório
 - Primeira vez
```bash
git push -u origin main
```
 - próximas vezes
```bash
git push
```
### Clonar um repositório
```bash
git clone <endereço do repositório na nuvem>
```

### Trazer modificações
```bash
git pull
```
### Gitignore
```bash
touch .gitignore
```

## Trabalho prático
 - Formar duplas
 - Git clone no repositório base
 - Apagar o repositório antigo
 - Integrante A subir o repositório base pra um repositório privado na nuvem
 - Integrante A tonrar integrante B colaborador (writer) do repositório na nuvem
 - Integrante A implementa função somar, roda no programa principal e sobe o código
 - Integrante B implementa função subtrair, roda no programa principal e sobe o código
 - Integrante A implementa função multiplicar, roda no programa principal e sobe o código
 - Integrante B implementa função divisão, roda no programa principal e sobe o código
 - Integrante A cria um conflito para o B resolver
 - Integrante B cria um conflito para o A resolver

## Apagar nossos rastros
### Deletar credenciais
 - Verificar antes
```bash
git config --list
```
 - Nome e email
```bash
git config --global user.name ""
```
```bash
git config --global user.email ""
```
 - Verificar depois
```bash
git config --list
```
Depois digite `q` para sair do modo de leitura.

### Deletar chave SSH local
```bash
start ~/.ssh
```
E deletar todos os arquivos da pasta.

## Well done! :tada::tada: