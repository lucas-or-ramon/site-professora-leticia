# 🚀 Guia Rápido de Início - Ballet Professor Website

## Passo 1: Personalizar o Site (5 minutos)

Abra o arquivo `index.html` com um editor de texto e procure por:

```
🔍 Substituir:
├── Logo: "Ballet Studio" → Seu nome
├── Seção Sobre: Texto padrão → Sua experiência
├── Turmas: Horários exemplos → Seus horários reais
├── Contato: Telefone/Email → Seus dados
└── Redes Sociais: Links placeholder → Seus perfis
```

**Exemplo rápido:**
```html
<!-- ANTES: -->
<div class="logo">🩰 Ballet Studio</div>

<!-- DEPOIS: -->
<div class="logo">🩰 Maria's Ballet</div>
```

## Passo 2: Adicionar Fotos (10 minutos)

1. **Coloque suas fotos** na pasta `/images/`
2. **Substitua os placeholders** no HTML:

```html
<!-- Procure por: -->
<img src="images/placeholder-1.jpg" alt="...">

<!-- E mude para: -->
<img src="images/minhas-fotos/aula-1.jpg" alt="Aula de ballet infantil">
```

**Dica:** Nomes de ficheiros:
- ✅ `aula-iniciante.jpg` (bom)
- ✅ `apresentacao-2024.jpg` (bom)
- ❌ `IMG_20240101.jpg` (evitar)

## Passo 3: Testar Localmente (2 minutos)

Se tem Python instalado:
```bash
cd /home/lucas-or-ramon/projetos/ballet-professor-website
python -m http.server 8000
```

Abra no navegador: **http://localhost:8000**

## Passo 4: Publicar no GitHub Pages (5 minutos)

### 4.1 Criar conta GitHub
- Vá para [github.com](https://github.com)
- Sign up (gratuito)
- Confirme email

### 4.2 Criar novo repositório
1. Clique no ➕ (canto superior direito)
2. "New repository"
3. Nome: `ballet-professor-website`
4. Público ✅
5. Clique "Create repository"

### 4.3 Enviar os arquivos

```bash
# No terminal, dentro da pasta do projeto:
git init
git config user.name "Seu Nome"
git config user.email "seu.email@gmail.com"
git add .
git commit -m "Primeiro commit - site ballet"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/ballet-professor-website.git
git push -u origin main
```

### 4.4 Ativar GitHub Pages

1. No GitHub, vá para seu repositório
2. **Configurações** → **Pages** (menu esquerdo)
3. Branch: selecione `main`
4. Pasta: `/` (root)
5. Clique **Save**

**Pronto! Seu site estará em:**
```
https://SEU_USUARIO.github.io/ballet-professor-website
```

## Passo 5: Configurar Formulário de Contato (3 minutos)

Atualmente, o formulário mostra uma mensagem de sucesso local.

Para **receber emails de verdade**:

1. Acesse [formsubmit.co](https://formsubmit.co)
2. Digite seu email
3. Copie o URL gerado
4. Abra `index.html`, procure por:
```html
<form class="contact-form" id="contactForm">
```
5. Substitua por:
```html
<form action="https://formsubmit.co/seu-email@example.com" method="POST">
```

**Altere:** `seu-email@example.com` pelo seu email real

## 📋 Checklist de Personalização

- [ ] Nome/Logo alterado
- [ ] Seção "Sobre" reescrita com suas informações
- [ ] Turmas atualizadas com seus horários
- [ ] Telefone e email atualizados
- [ ] Fotos adicionadas em `/images/`
- [ ] Imagens placeholder substituídas
- [ ] Vídeos adicionados (YouTube ou locais)
- [ ] Formulário de contato ativado (opcional)
- [ ] Testado no navegador (Chrome, Firefox, Safari)
- [ ] Testado no telefone/tablet
- [ ] Publicado no GitHub Pages

## 🎨 Mudar Cores

Abra `css/styles.css` e encontre:

```css
:root {
    --primary-color: #9b59b6;      /* roxo */
    --secondary-color: #e91e63;    /* rosa */
    --dark-color: #2c3e50;         /* cinza escuro */
}
```

**Paletas prontas para ballet:**

**Clássica:**
```css
--primary-color: #9b59b6;      /* Roxo */
--secondary-color: #e91e63;    /* Rosa pink */
```

**Sofisticada:**
```css
--primary-color: #7c3aed;      /* Violeta */
--secondary-color: #ec4899;    /* Magenta */
```

**Elegante:**
```css
--primary-color: #6d28d9;      /* Roxo escuro */
--secondary-color: #d946a6;    /* Orchid */
```

## 📧 Domínio Personalizado (Opcional)

Se quiser seu próprio domínio:

1. Compre em:
   - [Registro.br](https://www.registro.br) (domínios .br - ~R$30/ano)
   - [Namecheap](https://www.namecheap.com) (~$8/ano)

2. Configura no GitHub:
   - Go to Settings → Pages
   - Em "Custom domain" adicione seu domínio
   - Siga instruções de DNS

Exemplo: `meu-ballet.com.br` → seu site profissional!

## ⚡ Dicas de Performance

- **Comprimir imagens:** Use [tinypng.com](https://tinypng.com) antes de adicionar
- **Tamanho ideal:** 1200x800px para galeria
- **Formato:** JPG para fotos, PNG para gráficos

## 🆘 Problemas Comuns

**❓ "O site não aparece após publicar"**
- Espere 5-10 minutos para GitHub processar
- Pressione Ctrl+Shift+Delete para limpar cache

**❓ "As imagens não aparecem"**
- Verifique o caminho: `images/nome-correto.jpg`
- Reparar Case-sensitive (BallET.jpg ≠ ballet.jpg)

**❓ "Formulário não envia emails"**
- Confirme que usou FormSubmit.co
- Verifique pasta de Spam

## 📚 Recursos Úteis

- [HTML Tutorial](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS Tutorial](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [GitHub Pages Docs](https://pages.github.com)
- [Como usar Git](https://git-scm.com/doc)

## 🎉 Você está pronto!

Parabéns! Seu site está criado e pronto para personalizção. Qualquer dúvida sobre HTML/CSS, consulte os tutoriais acima.

**Próximas melhorias:**
- 📸 Blog com novidades
- 💳 Sistema de pagamento para inscrição
- 📅 Calendário dinâmico de disponibilidade
- 🔐 Área de alunos com senhas

Bom trabalho! 🩰
