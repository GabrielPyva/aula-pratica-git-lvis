# :octocat: Parte Prática da Aula de Git e GitHub

Bem-vindo(a) a parte prática da nossa aula de Git e GitHub! Este repositório foi criado para que você possa praticar os conceitos que vimos na aula de forma segura e guiada.

Nosso objetivo é simular um fluxo de trabalho colaborativo, onde cada um contribui com uma parte do projeto. Vamos lá!

### ✅ Pré-requisitos

Antes de começar, garanta que você tenha:
1.  O **[GitHub Desktop](https://desktop.github.com/)** instalado no seu computador.
2.  Um editor de código de sua preferência (ex: **[VS Code](https://code.visualstudio.com/)**).
3.  O **[interpretador de Python](https://www.python.org/)**

---

## 🎯 Parte 1: Sua Primeira Contribuição!

Nesta primeira parte, você irá criar um arquivo pessoal, fazer suas primeiras alterações e propor que elas sejam adicionadas ao projeto principal através de um Pull Request.

#### 1. Clonando o Repositório
Para começar, você precisa de uma cópia local deste projeto.

* No GitHub Desktop, vá em `File > Clone Repository...`.
* Selecione a aba `URL`.
* Cole a URL deste repositório (você pode pegá-la no botão verde "Code" aqui em cima).
* Escolha uma pasta no seu computador para salvar o projeto e clique em `Clone`.

#### 2. Criando sua Branch de Trabalho
Nunca trabalhamos diretamente na `main`! Vamos criar uma "ramificação" (branch) só sua.

* Na barra superior do GitHub Desktop, onde está escrito `Current Branch: main`, clique e depois no botão `New Branch`.
* Dê um nome para sua branch. Use o padrão `aluno/seu-nome` (ex: `aluno/joao-silva`).
* Clique em `Create Branch`.

#### 3. Criando seu Arquivo e Fazendo o Primeiro Commit
Agora é hora de criar seu código!

* Abra a pasta do projeto no seu editor de código (VS Code).
* Crie um novo arquivo com o nome `seu-nome.py` (ex: `joao-silva.py`).
* Dentro do arquivo, adicione o seguinte código, **substituindo pelo seu nome**:
    ```python
    # Autor: João da Silva
    print("Olá, mundo! Meu nome é João da Silva.")
    ```
* Salve o arquivo e volte para o GitHub Desktop. Você verá que sua alteração aparece na lista à esquerda!
* Para salvar essa "fotografia" do seu trabalho (o commit), preencha os campos no canto inferior esquerdo:
    * **Summary (obrigatório):** Escreva uma mensagem
    * **Description (opcional):** Dê mais detalhes se quiser.
* Clique no botão azul `Commit to aluno/seu-nome`.

#### 4. Publicando sua Branch
Seu commit está salvo, mas apenas no seu computador. Vamos enviá-lo para o GitHub.

* Clique no botão azul que agora diz `Publish branch`.

#### 5. Abrindo o Pull Request (PR)
Ótimo! Sua branch com seu código já está no repositório online. Agora, vamos pedir para que seu código seja adicionado à branch `main`.

* Após publicar, o GitHub Desktop geralmente mostra uma faixa azul com um botão `Create Pull Request`. Clique nele!
* Seu navegador vai abrir na página de criação do Pull Request. O título e a descrição já virão preenchidos.
* Apenas revise as informações e clique no botão verde `Create Pull Request`.

**🎉 Parabéns! Você acabou de criar seu primeiro Pull Request!**

---

## 🌪️ Parte 2: O Desafio do Trabalho em Equipe

Agora as coisas ficam interessantes. Vamos todos editar o *mesmo arquivo* e aprender a resolver conflitos que podem surgir.

#### 1. Sincronizando com a `main`
Antes de começar uma nova tarefa, sempre buscamos as atualizações mais recentes do projeto.

* No GitHub Desktop, mude sua branch atual de volta para a `main`.
* Clique no botão `Fetch origin` no topo. Isso busca as informações do repositório remoto.
* Se houverem atualizações, o botão mudará para `Pull origin`. Clique nele para baixar as novidades.

#### 2. Criando uma Nova Branch
Vamos criar uma nova branch para esta tarefa, a partir da `main` que acabamos de atualizar.

* Com a `main` selecionada, clique em `New Branch`.
* Dê um nome para a nova branch. Ex: `feature/adiciona-nome-lista`.

#### 3. Editando o Arquivo Compartilhado
* No seu editor de código, abra o arquivo `PARTICIPANTES.md`.
* Adicione seu nome completo ao final da lista.
* Salve o arquivo.
* Volte ao GitHub Desktop, faça o `commit` da sua alteração e dê `push` para o repositório remoto (clicando em `Push origin`).

#### 4. Resolvendo um Conflito de Merge!
O instrutor irá aceitar o Pull Request de um colega primeiro. Isso fará com que o seu PR entre em conflito, pois vocês dois editaram a mesma parte do mesmo arquivo! **Isso é normal!**

Quando o GitHub avisar do conflito, veja como resolver:

* No GitHub Desktop, com a sua branch `feature/adiciona-nome-lista` selecionada, vá no menu `Branch > Update from main`.
* O programa vai tentar fazer o merge e avisará que encontrou **1 conflicted file**.
* Ele te dará um botão `Open in Visual Studio Code` (ou seu editor padrão). Clique nele.
* Dentro do arquivo, você verá algo assim:
    ```
    <<<<<<< HEAD
    - Meu Nome Que Eu Adicionei
    =======
    - Nome do Colega que chegou antes
    >>>>>>> main
    ```
* **Sua missão:** Limpe o arquivo! Apague os marcadores (`<<<<<`, `=====`, `>>>>>`) e deixe o arquivo do jeito que ele deveria ser, com o nome do seu colega E o seu nome.
    ```
    - Nome do Colega que chegou antes
    - Meu Nome Que Eu Adicionei
    ```
* Salve o arquivo.
* Volte para o GitHub Desktop. A mensagem de conflito terá sumido! Clique no botão `Commit merge` para finalizar.
* Por último, clique em `Push origin` para enviar a resolução do conflito para o GitHub. Seu Pull Request estará pronto para ser aceito!

---

### ✨ Conclusão

Se você chegou até aqui, você:
* Clonou um repositório.
* Trabalhou em branches isoladas.
* Fez commits para salvar seu progresso.
* Abriu Pull Requests para propor mudanças.
* E o mais importante: **resolveu um conflito de merge como um(a) profissional!**

Essas são as habilidades essenciais para trabalhar em qualquer projeto de software em equipe. Parabéns!
