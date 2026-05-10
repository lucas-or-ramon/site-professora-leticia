# Ballet Studio - Website Estático

Um website elegante e responsivo para professora de ballet, desenvolvido com HTML5, CSS3 e JavaScript puro. Hospedagem 100% gratuita no GitHub Pages.

## 📂 Estrutura de Arquivos

```
ballet-professor-website/
├── index.html           # Página principal
├── css/
│   └── styles.css       # Estilos CSS
├── js/
│   └── script.js        # JavaScript interativo
├── images/              # Pasta para imagens (adicione suas fotos)
├── videos/              # Pasta para vídeos (se quiser hospedar localmente)
├── .gitignore           # Arquivo Git
└── README.md            # Este arquivo
```

## 🎯 Seções do Website

1. **Navegação** - Menu responsivo com links para todas as seções
2. **Hero** - Banner de boas-vindas com chamada principal
3. **Sobre** - Informações sobre a professora com estatísticas
4. **Turmas** - Descrição de todas as turmas disponíveis
5. **Galeria** - Espaço para fotos das aulas
6. **Vídeos** - Vídeos de apresentações e aulas
7. **Agenda** - Tabela com horários das aulas
8. **Contato** - Informações de contato e formulário

## 🚀 Como Usar

### 1️⃣ Personalizar o Conteúdo

Abra o arquivo `index.html` e atualize:

- **Seção "Sobre"** - Adicione informações sobre você
- **Turmas** - Modifique horários, descrições e disponibilidade
- **Contato** - Atualize telefone, email e endereço
- **Logo** - Substitua "🩰 Ballet Studio" pelo seu nome

```html
<!-- Exemplo: Alterar o nome -->
<div class="logo">Seu Nome - Ballet</div>
```

### 2️⃣ Adicionar Imagens

1. Coloque suas fotos na pasta `images/`
2. Substitua os nomes dos placeholders no HTML:

```html
<!-- De: -->
<img src="images/placeholder-1.jpg" alt="Descrição">

<!-- Para: -->
<img src="images/foto-aula-1.jpg" alt="Aula de ballet nível iniciante">
```

### 3️⃣ Adicionar Vídeos

**Opção A: YouTube (recomendado)**
```html
<iframe width="100%" height="400" 
    src="https://www.youtube.com/embed/ID_DO_VIDEO" 
    frameborder="0" allowfullscreen>
</iframe>
```

**Opção B: Arquivos locais**
```html
<video width="100%" controls>
    <source src="videos/apresentacao.mp4" type="video/mp4">
    Seu navegador não suporta a tag de vídeo.
</video>
```

### 4️⃣ Formulário de Contato

O formulário atualmente mostra uma mensagem de sucesso. Para receber emails, você tem 2 opções:

**Opção 1: FormSubmit.co (gratuito, recomendado)**
1. Acesse [formsubmit.co](https://formsubmit.co)
2. Configure seu email
3. Substitua no arquivo `js/script.js`:

```javascript
// Descomente e altere:
window.location.href = `mailto:seu-email@example.com...`;
```

**Opção 2: Formulário externo**
```html
<form action="https://formspree.io/f/SEU_ID" method="POST">
    <!-- campos do formulário -->
</form>
```

## 🌐 Hospedagem no GitHub Pages (Gratuito)

### Passo 1: Criar conta no GitHub
1. Vá para [github.com](https://github.com)
2. Crie uma conta gratuita

### Passo 2: Subir o projeto

```bash
# 1. Inicializar repositório
git init

# 2. Adicionar todos os arquivos
git add .

# 3. Fazer commit
git commit -m "Projeto Site Ballet"

# 4. Adicionar repositório remoto (substitua SEU_USUARIO)
git remote add origin https://github.com/SEU_USUARIO/ballet-professor-website.git

# 5. Enviar para GitHub
git branch -M main
git push -u origin main
```

### Passo 3: Ativar GitHub Pages

1. Vá para seu repositório no GitHub
2. Clique em **Settings** (Configurações)
3. Vá para **Pages** (no menu esquerdo)
4. Em "Source", selecione **main** e **/ (root)**
5. Clique **Save**

Seu site estará disponível em: `https://SEU_USUARIO.github.io/ballet-professor-website`

## 🎨 Personalizando as Cores

Abra `css/styles.css` e modifique as cores no topo:

```css
:root {
    --primary-color: #9b59b6;      /* Cor roxa (primária) */
    --secondary-color: #e91e63;    /* Cor rosa (secundária) */
    --dark-color: #2c3e50;         /* Cor escura */
    --light-color: #ecf0f1;        /* Cor clara */
}
```

**Sugestões de paletas para ballet:**
- Roxo clássico: `#9b59b6` e `#e91e63`
- Rosa sofisticado: `#d946a6` e `#ec4899`
- Violeta elegante: `#7c3aed` e `#a855f7`

## 📱 Para Visualizar Localmente

Se quiser testar antes de publicar:

```bash
# Com Python 3
python -m http.server 8000

# Com Python 2
python -m SimpleHTTPServer 8000

# Com Node.js (npm install -g http-server)
http-server
```

Acesse `http://localhost:8000` no navegador.

## ✉️ Configurar Emails de Contato

### Usando FormSubmit.co (Recomendado - Gratuito)

1. Acesse https://formsubmit.co
2. Digite seu email
3. Ele vai gerar um URL único para seu formulário
4. Adicione ao HTML:

```html
<form action="https://formsubmit.co/seu-email@example.com" method="POST">
    <input type="text" placeholder="Seu Nome" required>
    <input type="email" placeholder="Seu Email" required>
    <textarea placeholder="Mensagem" required></textarea>
    <button type="submit">Enviar</button>
</form>
```

## 💡 Dicas Importantes

✅ **Backup regularmente** - Guarde cópias do seu site
✅ **Atualize frequentemente** - Adicione novas fotos e vídeos
✅ **Use domínio personalizado** - Compre um domínio (cerca de R$30/ano) e configure no GitHub Pages
✅ **Teste no mobile** - Sempre visualize no celular antes de publicar
✅ **Otimize imagens** - Use ferramentas como TinyPNG para comprimir fotos

## 🔒 Domínio Personalizado (Opcional)

Para ter um domínio como `www.seunomedancas.com.br`:

1. Compre um domínio em:
   - [Registro.br](https://www.registro.br) (domínios .br)
   - [Namecheap](https://www.namecheap.com)
   - [Google Domains](https://domains.google)

2. Configure no GitHub Pages:
   - Settings → Pages
   - Em "Custom domain" adicione seu domínio
   - Siga as instruções de DNS do seu provedor

## 📧 Suporte

Para dúvidas sobre:
- **HTML/CSS/JS**: Consulte [MDN Web Docs](https://developer.mozilla.org)
- **GitHub**: [Documentação oficial do GitHub](https://docs.github.com)
- **GitHub Pages**: [Documentação oficial](https://pages.github.com)

## 📄 Licença

Este projeto é livre para uso pessoal e comercial.

---

**Desenvolvido com ❤️ para amor ao ballet** 🩰
