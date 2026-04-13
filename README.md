"Workshop-Git-Github" 

# 1 - Introdução ao Git e ao GitHub

Explicar primeiro o git

Depois o github

Ressaltar a diferença

# 2 - Como o Git e o Github são importantes

Comece mostrando o GitHub como uma plataforma de hospedagem de código, usando exemplos reais e famosos para engajar os participantes:

Acesse github.com/microsoft — mostre que grandes empresas hospedam seus projetos lá

Acesse github.com/microsoft/vscode — o próprio VS Code é open source e está no GitHub

Mostre estrelas, forks, commits e contribuidores para contextualizar a escala

# 3 - O Que é Git vs GitHub
Diferencie os dois conceitos antes de qualquer comando:

Git → ferramenta de controle de versão que roda localmente no seu computador

GitHub → plataforma online que hospeda repositórios Git e facilita colaboração

Analogia útil: Git é o sistema de salvamento; GitHub é a nuvem onde você faz backup e compartilha

3. Criando a pasta do Projeto
Abrir CMD e localizar onde voce esta

Criar uma pasta pelo CMD e entrar na mesma usando os comandos
mkdir 'Nome da pasta' PARA CRIAR PASTA
cd 'Nome da pasta' PARA ENTRAR NA PASTA

4. Diferenciar uma pasta simples com um repositório local
Ao abrir a pasta mostrar que não existe nada (De forma simples e Tecnica)
Iniciar o Repositorio local com o comando
git init
Explicar que a pasta criada se tornou um Repositorio local

5. Criando o Projeto
Abrir o VS Code no CMD com o comando
code .

Crie um arquivo index.html básico dentro do VS Code

6. Fluxo de Commit
Explique os 3 estados de um arquivo no Git antes dos comandos:

Estado	Descrição
Untracked	Git não monitora o arquivo ainda
Staged	Arquivo adicionado, pronto para commit (git add)
Committed	Versão salva no histórico local

Mostrar na pratica os comandos
git status 'Mostrar os arquivos untracked'
git add index.html  'Move para staged'

E novamente dar um git status para mostrar que o arquivo agora esta sendo rastreado e pronto para ser comitado

7. Indentificar usuario
Antes precisamos Identificar-se antes do primeiro commit com os comandos

git config --global user.name "seu usuario"
git config --global user.email "seu email"

Os mesmos usados no GitHub

8. Hora de efetuar o commit

Agora vamos efetuar nosso primeiro commit e inserir uma mensagem com as alterações feitas com o comando
git commit -am "Mensagem do usuario" 

9. Conectando ao Repositório Remoto
Vamos conectar Repositorio ao remoto no GitHub com o comando
git remote add origin 'Link do Repositorio criado'
Em seguida vamos verificar se foi criado seu Repositorio remoto com o comando
git remote -v

10. Atenticação com Token(PTA)
Como gerar o PAT:

GitHub → foto de perfil → Settings

Developer settings → Personal access tokens → Tokens (classic)

Generate new token → dê um nome descritivo

Marque o escopo repo (controle total de repositórios)

Clique em Generate token e copie imediatamente (só aparece uma vez)

Quando dar o push vai pedir o PTA

 Username: seu usuario
 Password: (cole o token aqui)

11. Push
Agora podemos efetuar no Push para subir os arquivos para o GitHub com o comando
git push origin main

12. Pull
Com o comando git pull origin main
Baixamos as mudanças feitas no Repositorio remoto
