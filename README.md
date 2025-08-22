# 🌱 Guia para Iniciantes em Git e GitHub

Bem-vindo ao tutorial mais completo e didático de Git/GiHub para iniciantes absolutos! Este material foi criado especialmente para quem nunca trabalhou com versionamento de código e quer aprender de forma prática e divertida.

## 1 Introdução
### 1.1. O que é o Git?
Pense no `Git` como a “máquina do tempo” do seu projeto.
Ele guarda cada versão do seu código, permitindo que você volte no tempo, compare mudanças e trabalhe em equipe sem bagunça.

Imagine que você está escrevendo um livro no Word e cada vez que muda algo, você salva o arquivo como `livro_v1.docx`, `livro_v2.docx`, `livro_final_agora_sim.docx`.
O Git automatiza esse processo e organiza todas essas versões de forma inteligente.

### 1.2. O que é o GitHub?
O `GitHub` é como o Google Drive para projetos com Git.
Você armazena seu repositório na nuvem e pode compartilhar com outras pessoas para colaborar.

Git é a sua mochila com os cadernos (versões do projeto).
GitHub é a estante da biblioteca onde você pode guardar e compartilhar essa mochila com os colegas.

### 1.3. Instalando o Git
Se ainda não tiver o Git instalado:
👉 [Baixe aqui](https://git-scm.com/downloads)

Após instalar, configure seu usuário (uma vez só no PC):
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"
```

## 2. Seu Primeiro Repositório
Vamos criar um repositório local (na sua máquina):
```bash
# Criar uma pasta
mkdir meu-projeto
cd meu-projeto

# Iniciar o git
git init
```
Agora temos um repositório Git inicializado.

Você comprou um caderno novo (projeto) e colocou a etiqueta com seu nome (git init).
A partir de agora, cada página escrita pode ser guardada como uma versão.

## 3. Ciclo Básico do Git
O ciclo do Git costuma ser simples e dividido em 3 etapas:
`Escreve` → altera ou cria arquivos
`Marca` → adiciona ao controle do Git (`git add`)
`Fotografa` → registra um ponto na linha do tempo (`git commit`)

Exemplo:
```bash
echo "Hello Git!" > app.txt     # Criar arquivo
git add app.txt                 # Marcar para salvar
git commit -m "Primeira versão" # Fotografar
```

Onde teríamos algo como:
`git add` = Colocar as páginas na “caixa de fotos”
`git commit` = Tirar a foto oficial e guardar no álbum do projeto

## 4. Histórico
Quer ver as "fotos" já tiradas (`commits`)?
```bash
git log --oneline
```

## 5. Conectando ao GitHub
Para iniciarmos, assista essa vídeo aula:

<a href="https://www.youtube.com/watch?v=NUHs75BrQtg" target="_blank"><img height="168" width="300" src="https://i.ytimg.com/vi/NUHs75BrQtg/hqdefault.jpg?sqp=-oaymwEnCPYBEIoBSFryq4qpAxkIARUAAIhCGAHYAQHiAQoIGBACGAY4AUAB&rs=AOn4CLCjfjWxHLQF6ouNPdHtav9JzsKlkg" target="_blank"></a>


Depois de você ter criado seu projeto local, criado seu repositório no GitHub e vinculado sua chave ssh-key, conecte seu projeto local ao repositório assim:
```bash
git remote add origin https://github.com/seuusuario/meu-projeto.git
git branch -M main
git push -u origin main
```
Lembra da mochila que falamos lá em cima? Agora você guardou sua mochila de anotações na estante (GitHub). Agora todos podem ver (se você quiser).

## 6. Atualizando o Projeto
Após você fazer alterações no seu projeto local, você confirma dessa forma:
```bash
git add .
git commit -m "Adicionei nova funcionalidade"
git push
```

Isso envia as mudanças para o GitHub.

## 7. Baixando Atualizações
Se o seu colega que também tem acesso ao repositório do Github enviou alguma atualização e você gostaria de atualizar seu projeto local com as alterações que ele fez, você atualiza assim:
```bash
git pull
```

É tipo ir na biblioteca e trazer a versão mais nova de um livro para casa.

## 8. Trabalhando em equipes: as Branches
Branches são "linhas do tempo alternativas" para desenvolver sem bagunçar o principal.
É como fazer uma cópia do livro para rascunho. Depois que o rascunho está bom, você junta no livro oficial.

```bash
git checkout -b nova-funcionalidade
```

Trabalhe, faça commits e depois junte com o principal (merge):

```bash
git checkout main
git merge nova-funcionalidade
```

## 9. Resumindo o Fluxo 🚦
- Cria/edita arquivos
- `git add` → Marca mudanças
- `git commit -m "msg"` → Salva versão
- `git push` → Envia para o GitHub
- `git pull` → Atualiza da nuvem

## 10. Dicas para Bons Commits
Mensagens curtas e claras:
- ✅ "Corrige bug no login"
- ❌ "alterei algumas coisas"

Faça commits frequentes, mas com sentido!

## 🎉 Vamos Começar!
DESAFIO
- Crie um repositório local chamado meu-blog
- Adicione um arquivo index.html com “Olá Mundo”
- Faça git add e git commit
- Crie o repositório no GitHub e faça git push
- Modifique o HTML e atualize no GitHub
- Pronto! 🎉 Você já está versionando seu primeiro projeto.

**Lembre-se**: Todo programador experiente já foi iniciante um dia. O importante é começar! 🚀

---

*Feito com ❤️ pelo professor [Bruno Batista]*(https://github.com/batistabjs)
