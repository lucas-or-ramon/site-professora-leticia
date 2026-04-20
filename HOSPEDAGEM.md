# 🌐 Como Hospedar no GitHub Pages (Gratuito)

Este guia mostra como publicar seu site Ballet Professor no GitHub Pages com **custo zero**.

## ✅ Requisitos

- Conta no [GitHub.com](https://github.com) (gratuita)
- Git instalado no seu computador
- Seu projeto pronto em `/home/lucas-or-ramon/projetos/ballet-professor-website`

## 📋 Passo a Passo

### 1️⃣ Criar Conta no GitHub

1. Vá para [github.com/signup](https://github.com/signup)
2. Preencha:
   - Email
   - Senha
   - Username (ex: `maria-ballet`, `ballet-teacher`, etc)
3. Confirme seu email

### 2️⃣ Inicializar Repositório Git

Abra o terminal e execute:

```bash
# Navegar para a pasta do projeto
cd /home/lucas-or-ramon/projetos/ballet-professor-website

# Inicializar git
git init

# Configurar seu nome e email (use os da sua conta GitHub)
git config user.name "Seu Nome"
git config user.email "seu-email@gmail.com"

# Verificar se funcionou
git config --list
```

### 3️⃣ Fazer Primeiro Commit

```bash
# Adicionar todos os arquivos
git add .

# Fazer commit
git commit -m "Projeto site - ballet professor"

# Renomear branch para 'main' (GitHub padrão)
git branch -M main
```

### 4️⃣ Criar Repositório no GitHub

1. Faça login no [GitHub.com](https://github.com)
2. Clique no ➕ canto superior direito
3. "New repository"
4. Preencha:
   - **Repository name:** `ballet-professor-website`
   - **Description:** Website para aulas de ballet (opcional)
   - **Public** ✅ (deve ser público para GitHub Pages)
   - Deixe as outras opções como estão
5. Clique **Create repository**

### 5️⃣ Conectar Repositório Local ao Remoto

Copie o HTTPS do seu repositório (na cor azul) e execute:

```bash
# Substitua USUARIO pelo seu username do GitHub
git remote add origin https://github.com/USUARIO/ballet-professor-website.git

# Verificar
git remote -v
```

### 6️⃣ Fazer Push para o GitHub

```bash
# Enviar código para GitHub
git push -u origin main
```

Se pedir senha, gere um token de acesso (em vez de usar senha):
[Como gerar token GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

### 7️⃣ Ativar GitHub Pages

1. No [GitHub.com](https://github.com), vá para seu repositório
2. Clique em **Settings** (Configurações)
3. No menu esquerdo, clique **Pages**
4. Em "Build and deployment":
   - **Source:** Deploy from a branch
   - **Branch:** Selecione `main`
   - **Folder:** `/` (root)
5. Clique **Save**

### 8️⃣ Aguardar Publicação

GitHub processará em até 5-10 minutos.

Seu site estará disponível em:
```
https://USUARIO.github.io/ballet-professor-website
```

❗ **Nota:** Troque `USUARIO` pelo seu username do GitHub

## 🔄 Fazer Atualizações no Futuro

Sempre que quiser atualizar:

```bash
# Fazer alterações no projeto...

# Adicionar mudanças
git add .

# Fazer commit
git commit -m "Descrição das mudanças"

# Enviar para GitHub
git push
```

Seu site será atualizado automaticamente!

## 🚀 Testar Antes de Publicar

Quando quiser testar localmente antes de publicar:

```bash
# Com Python 3
python -m http.server 8000

# Com Python 2
python -m SimpleHTTPServer 8000

# Com Node.js (instale com: npm install -g http-server)
http-server
```

Depois abra: `http://localhost:8000`

## 🎯 Adicionar Domínio Personalizado (Opcional)

Se quer um domínio próprio como `www.meu-ballet.com.br`:

### Compra do Domínio

1. Compre em:
   - [Registro.br](https://www.registro.br) - Domínios .br
   - [Namecheap](https://www.namecheap.com) - Domínios internacionais
   - [Google Domains](https://domains.google)

2. Custo aproximado:
   - Domínios .br: ~R$30/ano
   - Outros domínios: $8-15 USD/ano

### Configuração no GitHub Pages

1. No GitHub, vá para Settings → Pages
2. Em "Custom domain", digite seu domínio
3. Clique **Save**
4. Você receberá instruções de DNS
5. Configure no painel de controle do seu registrador de domínio

Exemplo de configuração DNS:
- `A` records apontando para IPs do GitHub
- `CNAME` apontando para `seu-usuario.github.io`

[Documentação oficial GitHub Pages](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## ✅ Checklist Final

- [ ] Conta GitHub criada
- [ ] Repositório criado no GitHub
- [ ] Git inicializado localmente
- [ ] Código feito push para GitHub
- [ ] GitHub Pages ativado
- [ ] Site acessível em `https://usuario.github.io/ballet-professor-website`
- [ ] Website testado em desktop, tablet e mobile
- [ ] Formulário de contato (opcional) configurado
- [ ] Domínio personalizado (opcional) configurado

## 🆘 Problemas Comuns

### ❌ "Repository not found"
**Solução:** Verifique se o repositório é público (Settings → General)

### ❌ "The site hasn't been published yet"
**Solução:** Aguarde 10-15 minutos. GitHub pode ser lento. Atualize a página.

### ❌ "fatal: not a git repository"
**Solução:** Execute `git init` na pasta correta do projeto

### ❌ "fatal: permission denied"
**Solução:** Use token de acesso em vez de senha
[Gerar token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

## 💡 Benefícios do GitHub Pages

✅ **Gratuito** - Sem custos mensais
✅ **Sempre Online** - 99.9% de uptime
✅ **HTTPS** - Segurança garantida
✅ **Rápido** - CDN global
✅ **Controle de Versão** - Git integrado
✅ **Contínuo** - Atualizações automáticas
✅ **Escalável** - Suporta muito tráfego

## 📚 Recursos Adicionais

- [Documentação GitHub Pages](https://pages.github.com)
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
- [Como usar GitHub](https://github.com/skills)

---

**Pronto!** Seu site está no ar 24/7, 365 dias por ano, completamente gratuito! 🩰🌐
