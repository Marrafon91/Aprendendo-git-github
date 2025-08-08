<h1 align="center">📌 Cola Git Bash – Principais Comandos</h1>

<p align="center">
Guia rápido com os comandos mais usados no <b>Git</b> para você consultar e trabalhar de forma mais produtiva.
</p>

---

## 🛠️ Configuração Inicial
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```
Define seu nome e email no Git (necessário para identificar seus commits).  
O `--global` significa que vale para todos os repositórios do seu computador.

```bash
git config --list
```
Mostra todas as configurações atuais do Git.

---

## 📂 Criar e Clonar Repositórios
```bash
git init
```
Cria um repositório Git vazio na pasta atual.

```bash
git clone URL
```
Clona um repositório existente para seu computador.  
Exemplo:
```bash
git clone https://github.com/usuario/repositorio.git
```

---

## 📜 Status e Histórico
```bash
git status
```
Mostra o estado atual do repositório (arquivos modificados, novos, prontos para commit).

```bash
git log
```
Mostra o histórico de commits.

```bash
git log --oneline
```
Mostra o histórico de commits de forma resumida.

---

## 📌 Adicionar e Salvar Alterações
```bash
git add arquivo.txt
```
Adiciona **um arquivo específico** para o próximo commit.

```bash
git add .
```
Adiciona **todos os arquivos modificados** para o próximo commit.

```bash
git commit -m "mensagem do commit"
```
Salva as mudanças adicionadas com uma mensagem descritiva.

---

## 🔄 Enviar e Receber Alterações
```bash
git push origin main
```
Envia seus commits para o repositório remoto (branch `main`).

```bash
git pull origin main
```
Baixa e integra as alterações do repositório remoto para sua branch local.

---

## 🌿 Branches (Ramificações)
```bash
git branch
```
Lista todas as branches e indica a branch atual.

```bash
git branch nome-da-branch
```
Cria uma nova branch.

```bash
git checkout nome-da-branch
```
Muda para outra branch.

```bash
git checkout -b nome-da-branch
```
Cria **e já muda** para a nova branch.

```bash
git merge nome-da-branch
```
Junta as alterações de uma branch na branch atual.

---

## 🗑️ Desfazer Alterações
```bash
git restore arquivo.txt
```
Descarta modificações feitas em um arquivo **antes do `git add`**.

```bash
git reset HEAD arquivo.txt
```
Remove um arquivo da área de preparação (`git add`), mantendo as mudanças no arquivo.

```bash
git reset --hard
```
⚠️ **Cuidado:** volta todo o repositório para o último commit, descartando todas as alterações.

---

## 📦 Outros Comandos Úteis
```bash
git remote -v
```
Mostra os repositórios remotos configurados.

```bash
git stash
```
Salva alterações não commitadas temporariamente e limpa o diretório de trabalho.

```bash
git stash pop
```
Recupera as alterações salvas com `git stash`.

---

<h3 align="center">💡 Dicas importantes:</h3>

<p align="center">
<code>origin</code> → nome padrão do repositório remoto. <br>
<code>main</code> ou <code>master</code> → branch principal. <br>
Sempre rode <code>git status</code> antes de qualquer ação.
</p>
