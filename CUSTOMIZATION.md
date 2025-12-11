# 🎨 Guia de Customização

## 1️⃣ Adicionar Sua Foto

### Passo 1: Preparar a Imagem
1. Tire ou escolha uma foto profissional (quadrada, 400x400px recomendado)
2. Redimensione usando [Tinypng.com](https://tinypng.com) ou similar
3. Nomeie como `avatar.jpg`
4. Coloque na pasta `assets/`

### Passo 2: Adicionar ao HTML
No `portifolio.html`, adicione na seção hero:

```html
<div class="hero-content">
    <img src="assets/avatar.jpg" alt="Aline Daiane Carneiro" class="avatar">
    <h1>Aline Daiane Carneiro</h1>
    <!-- ... -->
</div>
```

### Passo 3: Estilizar no CSS
No `style.css`, adicione:

```css
.avatar {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    object-fit: cover;
    border: 4px solid var(--white);
    margin-bottom: 2rem;
    animation: slideInDown 0.8s ease;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
}

@media (max-width: 768px) {
    .avatar {
        width: 120px;
        height: 120px;
    }
}
```

---

## 2️⃣ Alterar Cores Principais

### No `style.css`, encontre:

```css
:root {
    --primary-color: #6366f1;      /* Mude para sua cor */
    --secondary-color: #8b5cf6;
    --accent-color: #ec4899;
    /* ... */
}
```

### Sugestões de Paletas:

**Azul Profissional:**
```css
--primary-color: #0066cc;
--secondary-color: #0052a3;
--accent-color: #ff6b6b;
```

**Verde Moderno:**
```css
--primary-color: #10b981;
--secondary-color: #059669;
--accent-color: #f59e0b;
```

**Roxo Elegante:**
```css
--primary-color: #7c3aed;
--secondary-color: #6d28d9;
--accent-color: #ec4899;
```

**Laranja Quente:**
```css
--primary-color: #f97316;
--secondary-color: #ea580c;
--accent-color: #06b6d4;
```

---

## 3️⃣ Adicionar Seção de Projetos

### Crie um novo arquivo `projetos.html` ou adicione ao HTML:

```html
<!-- Antes da seção #contato -->
<section id="projetos" class="projetos">
    <div class="container">
        <h2>Meus Projetos</h2>
        <div class="projetos-grid">
            
            <div class="projeto-card">
                <div class="projeto-imagem" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);"></div>
                <h3>Meu Primeiro Site</h3>
                <p>Desenvolvido durante o curso de Programação Web no Senac.</p>
                <div class="projeto-tags">
                    <span>HTML5</span>
                    <span>CSS3</span>
                    <span>JavaScript</span>
                </div>
                <div class="projeto-links">
                    <a href="https://github.com" target="_blank" class="btn btn-secondary">Ver no GitHub</a>
                    <a href="https://seu-site.com" target="_blank" class="btn btn-primary">Demo</a>
                </div>
            </div>

            <div class="projeto-card">
                <div class="projeto-imagem" style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);"></div>
                <h3>Calculadora JavaScript</h3>
                <p>Aplicação interativa com operações matemáticas avançadas.</p>
                <div class="projeto-tags">
                    <span>JavaScript</span>
                    <span>HTML5</span>
                    <span>CSS3</span>
                </div>
                <div class="projeto-links">
                    <a href="https://github.com" target="_blank" class="btn btn-secondary">Ver no GitHub</a>
                    <a href="#" target="_blank" class="btn btn-primary">Demo</a>
                </div>
            </div>

        </div>
    </div>
</section>
```

### Adicione ao CSS:

```css
.projetos {
    padding: 6rem 0;
    background: var(--white);
}

.projetos h2 {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 3rem;
}

.projetos-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: 2rem;
}

.projeto-card {
    background: var(--light-bg);
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 2px 15px rgba(0, 0, 0, 0.1);
    transition: var(--transition);
}

.projeto-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 30px rgba(99, 102, 241, 0.2);
}

.projeto-imagem {
    width: 100%;
    height: 200px;
    background-size: cover;
    background-position: center;
}

.projeto-card h3 {
    padding: 1.5rem 1.5rem 0.5rem;
    color: var(--text-dark);
}

.projeto-card p {
    padding: 0 1.5rem 1rem;
    color: var(--text-light);
    font-size: 0.9rem;
}

.projeto-tags {
    padding: 0 1.5rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 1rem;
}

.projeto-tags span {
    background: var(--white);
    padding: 0.3rem 0.8rem;
    border-radius: 20px;
    font-size: 0.8rem;
    color: var(--primary-color);
    border: 1px solid var(--primary-color);
}

.projeto-links {
    padding: 0 1.5rem 1.5rem;
    display: flex;
    gap: 1rem;
}

.projeto-links .btn {
    flex: 1;
    text-align: center;
    font-size: 0.9rem;
    padding: 0.8rem;
}
```

### Atualize o menu de navegação:

```html
<li><a href="#projetos">Projetos</a></li>
```

---

## 4️⃣ Integrar Formulário de Email Real

### Opção 1: Formspree (Recomendado)

1. Acesse [Formspree.io](https://formspree.io)
2. Faça login/cadastro
3. Crie um novo formulário
4. Copie o endpoint fornecido

5. No `portifolio.html`, atualize o form:

```html
<form class="contato-form" action="https://formspree.io/f/seu-id" method="POST" id="contactForm">
    <!-- campos existentes -->
</form>
```

### Opção 2: EmailJS

1. Acesse [EmailJS.com](https://www.emailjs.com)
2. Crie uma conta e configure
3. No `script.js`, adicione:

```javascript
emailjs.init('sua-public-key');

const contactForm = document.getElementById('contactForm');
if (contactForm) {
    contactForm.addEventListener('submit', (e) => {
        e.preventDefault();
        
        emailjs.sendForm('service_id', 'template_id', contactForm)
            .then((response) => {
                alert('Email enviado com sucesso!');
                contactForm.reset();
            }, (error) => {
                alert('Erro ao enviar: ' + error.text);
            });
    });
}
```

---

## 5️⃣ Ativar Dark Mode Completo

No `style.css`, adicione:

```css
body.dark-mode {
    --primary-color: #818cf8;
    --text-dark: #f1f5f9;
    --text-light: #cbd5e1;
    background-color: #0f172a;
}

body.dark-mode .navbar {
    background: #1e293b;
}

body.dark-mode .skill-card,
body.dark-mode .formacao-card,
body.dark-mode .info-item {
    background: #1e293b;
    color: #f1f5f9;
}

/* Mais estilos dark mode conforme necessário */
```

---

## 6️⃣ Adicionar Analytics

No `portifolio.html`, antes do `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_ID');
</script>
```

Substitua `GA_ID` pelo seu ID do Google Analytics.

---

## 7️⃣ Otimizar para SEO

No `portifolio.html`, atualize o `<head>`:

```html
<meta name="description" content="Portfólio de Aline Daiane - Profissional em Transição para Desenvolvimento Web">
<meta name="keywords" content="programação, web development, portfólio, currículo">
<meta name="author" content="Aline Daiane Carneiro">
<meta property="og:title" content="Aline Daiane Carneiro - Portfólio">
<meta property="og:description" content="Profissional em Transição para Desenvolvimento Web">
<meta property="og:image" content="https://seu-site.com/assets/avatar.jpg">
<meta property="og:url" content="https://seu-site.com">
```

---

## 8️⃣ Certificados e Badges

Adicione após a seção de formação:

```html
<section id="certificados" class="certificados">
    <div class="container">
        <h2>Certificados</h2>
        <div class="certificados-grid">
            <div class="certificado-card">
                <i class="fas fa-certificate"></i>
                <h3>Programação Web</h3>
                <p>Senac PR - 2025</p>
                <a href="#" target="_blank" class="btn btn-secondary">Visualizar</a>
            </div>
        </div>
    </div>
</section>
```

---

## ✨ Dicas Finais

1. **Mantenha o portfólio atualizado** - Atualize regularmente com novos projetos
2. **Use links reais** - Certifique-se que todos os links funcionam
3. **Imagens otimizadas** - Use ferramentas como [Tinypng](https://tinypng.com)
4. **Mobile first** - Teste sempre em dispositivos móveis
5. **Backup** - Sempre guarde cópias dos seus arquivos

---

**Precisa de ajuda?** Consulte a documentação ou abra uma issue no repositório!
