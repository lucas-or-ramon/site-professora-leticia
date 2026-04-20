# 📦 Estrutura do Projeto - Ballet Professor Website

```
ballet-professor-website/
│
├── 📄 index.html                    ← Página principal (EDITAR COM SEUS DADOS)
├── 📄 README.md                     ← Documentação completa
├── 📄 GUIA-RAPIDO.md               ← Guia de 5 passos para começar
├── 📄 HOSPEDAGEM.md                ← Como publicar no GitHub Pages
├── 📄 .gitignore                   ← Arquivos a ignorar no Git
│
├── 📁 css/
│   └── 📄 styles.css               ← Estilos CSS (cores, layouts)
│
├── 📁 js/
│   └── 📄 script.js                ← JavaScript (menu mobile, formulário, animações)
│
├── 📁 images/                       ← Suas fotos aqui
│   └── 📄 README.md                ← Instruções de imagens
│
├── 📁 videos/                       ← Seus vídeos aqui (ou links do YouTube)
│
└── 📁 .github/
    └── 📄 copilot-instructions.md  ← Notas do GitHub Copilot
```

## 🎯 O Que Está Incluído

### ✅ Site Completo com 8 Seções:
1. **Navegação** - Menu responsivo com hamburguer mobile
2. **Hero** - Banner de boas-vindas atrativo
3. **Sobre** - Apresentação da professora com estatísticas
4. **Turmas** - Cards com todas as turmas disponíveis
5. **Galeria** - Grid de imagens com efeito hover
6. **Vídeos** - Espaço para vídeos (YouTube ou locais)
7. **Agenda** - Tabela de horários bem formatada
8. **Contato** - Informações + formulário

### ✅ Recursos Implementados:
- 📱 **Responsivo** - Funciona em celular, tablet e desktop
- 🎨 **Moderno** - Design elegante com gradientes
- ⚡ **Rápido** - Zero dependências, sem frameworks
- 🔐 **Seguro** - Sem banco de dados, apenas arquivos estáticos
- 🎭 **Interativo** - Menu mobile, formulário, animações
- 🔍 **SEO** - Meta tags e estrutura semântica

## 🚀 Primeiros Passos

### 1. Personalizar Conteúdo (5 min)
```bash
# Abra index.html em um editor de texto
# Procure e substitua:
# - "Ballet Studio" → Seu nome
# - Horários das turmas
# - Telefone e email
# - Descrição pessoal
```

### 2. Adicionar Suas Fotos (10 min)
```bash
# Coloque suas fotos em: /images/
# Substitua os placeholders no HTML
# Dica: Comprima imagens em tinypng.com primeiro
```

### 3. Testar Localmente (2 min)
```bash
cd /home/lucas-or-ramon/projetos/ballet-professor-website
python -m http.server 8000
# Abra: http://localhost:8000
```

### 4. Publicar no GitHub Pages (5 min)
```bash
# Crie conta em github.com
# Faça upload do projeto
# Ative GitHub Pages em Settings
# Seu site estará em: https://seu-usuario.github.io/ballet-professor-website
```

Veja **GUIA-RAPIDO.md** para mais detalhes!

## 🌐 Hospedagem: Zero Custo!

| Aspecto | GitHub Pages |
|---------|-------------|
| **Custo** | 🎉 GRATUITO |
| **Uptime** | ✅ 99.9% |
| **HTTPS** | ✅ Sim |
| **Domínio** | Grátis ou personalizado |
| **Banda** | ✅ Ilimitada |
| **Atualizações** | Automáticas |

Veja **HOSPEDAGEM.md** para instruções passo a passo!

## 📊 Características Técnicas

```
🔧 Stack Tecnológico:
├── HTML5 (estrutura)
├── CSS3 com variáveis CSS
│   ├── Grid Layout
│   ├── Flexbox
│   └── Media Queries (responsivo)
├── JavaScript Vanilla
│   ├── Menu hamburguer
│   ├── Validação de formulário
│   ├── Animações ao scroll
│   └── Interatividade geral
└── 0 dependências externas!
```

## 🎨 Personalização

### Mudar Cores
```css
/* Em css/styles.css, procure por: */
:root {
    --primary-color: #9b59b6;      /* Roxo - mude aqui */
    --secondary-color: #e91e63;    /* Rosa - mude aqui */
    --dark-color: #2c3e50;
    --light-color: #ecf0f1;
}
```

**Sugestões para ballet:**
- Roxo clássico: `#9b59b6` + `#e91e63`
- Violeta moderno: `#7c3aed` + `#ec4899`
- Magenta elegante: `#d946a6` + `#a855f7`

### Adicionar Seções
O HTML é bem estruturado e fácil de modificar. Copie uma seção existente e adapte!

## 📧 Email (Formulário de Contato)

Atualmente mostra mensagem local. Para receber emails:

1. Acesse [formsubmit.co](https://formsubmit.co)
2. Copie o URL gerado
3. Substitua no HTML:
```html
<form action="https://formsubmit.co/seu-email@example.com" method="POST">
```

## 🔒 Domínio Personalizado (Opcional)

Para ter um domínio como `seu-ballet.com.br`:

1. Compre em:
   - [Registro.br](https://www.registro.br) (~R$30/ano)
   - [Namecheap](https://www.namecheap.com) (~$8/ano)
2. Configure em GitHub Pages Settings → Custom domain
3. Pronto!

## ✨ Destaques

- 🎯 **Pronto para uso** - Não precisa de configuração compleja
- 📱 **Mobile first** - Testa-se em celular primeiro
- ⚡ **Performance** - Carrega em menos de 1 segundo
- 🔍 **SEO básico** - Tags meta e estrutura semântica
- 📊 **Estatísticas** - Contador animado de experiência
- 🎬 **Galeria bonita** - Efeitos hover e responsiva
- 📅 **Agenda clara** - Tabela organizada de horários
- 📞 **Contato fácil** - Várias formas de entrar em contato

## 📚 Próximos Passos (Opcional)

- [ ] 📝 Adicionar blog com novidades
- 💳 Sistema de pagamento para inscrição
- 📈 Google Analytics para estatísticas
- 🔐 Área de alunos com senhas
- 📱 App mobile
- 💬 Live chat com alunos

## 📖 Documentação

| Arquivo | Descrição |
|---------|-----------|
| **README.md** | Documentação completa do projeto |
| **GUIA-RAPIDO.md** | Primeiros 5 passos (comece aqui!) |
| **HOSPEDAGEM.md** | Como publicar no GitHub Pages |
| **index.html** | Página principal comentada |
| **css/styles.css** | CSS comentado com variáveis |
| **js/script.js** | JavaScript comentado |

## 🆘 Precisa de Ajuda?

- [MDN Web Docs](https://developer.mozilla.org) - Para HTML/CSS/JS
- [GitHub Docs](https://docs.github.com) - Para Git e GitHub Pages
- [Stack Overflow](https://stackoverflow.com) - Para dúvidas técnicas

## 🎉 Você Está Pronto!

Seu site de ballet está 100% pronto. Só falta personalizar com suas informações e fotos!

**Comece pelo:** [GUIA-RAPIDO.md](GUIA-RAPIDO.md)

---

**Desenvolvido com ❤️ para amor ao ballet**  
Hospedado gratuitamente no GitHub Pages 🩰
