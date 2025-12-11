# 👋 Portfólio - Aline Daiane Carneiro

[![HTML5](https://img.shields.io/badge/HTML5-E34C26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> Portfólio profissional moderno e responsivo de **Aline Daiane Carneiro** - Profissional em Transição para Desenvolvimento Web

## 📋 Conteúdo

- [Sobre](#-sobre)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Como Usar](#-como-usar)
- [Personalização](#-personalização)
- [Funcionalidades](#-funcionalidades)
- [Deploy](#-deploy)
- [Contato](#-contato)

## 🎯 Sobre

Este é um portfólio profissional completo desenvolvido com **HTML5, CSS3 e JavaScript vanilla**. O site apresenta:

- **Experiência Profissional**: Trajetória como Consultora de Cobrança e Auxiliar Administrativo
- **Formação Acadêmica**: Bacharelado em Ciência da Computação (PUC-PR) e Formação em Programação Web (Senac)
- **Competências**: Trabalho em equipe, negociação, comunicação, programação lógica e atendimento ao cliente
- **Design Responsivo**: Funciona perfeitamente em desktop, tablet e mobile

## 🛠️ Tecnologias Utilizadas

### Front-end
- **HTML5** - Estrutura semântica
- **CSS3** - Estilos modernos com Flexbox e Grid
- **JavaScript (Vanilla)** - Interatividade e animações
- **Font Awesome** - Ícones profissionais

### Recursos
- Design Responsivo (Mobile-first)
- Animações Suaves
- Navegação Intuitiva
- Formulário de Contato
- Scroll Suave
- Lazy Loading de Imagens
- Dark Mode (Preparado)

## 📁 Estrutura do Projeto

```
portifolio_Aline/
├── portifolio.html      # Arquivo principal HTML
├── style.css            # Estilos CSS
├── script.js            # Lógica JavaScript
├── README.md            # Este arquivo
└── assets/              # Pasta para imagens (opcional)
    └── logo.png
```

## 🚀 Como Usar

### 1. **Clonar o Repositório**
```bash
git clone https://github.com/seu-usuario/portifolio_Aline.git
cd portifolio_Aline
```

### 2. **Abrir Localmente**
Simply open `portifolio.html` em seu navegador:
```bash
# Windows
start portifolio.html

# macOS
open portifolio.html

# Linux
xdg-open portifolio.html
```

### 3. **Usar com Live Server (Recomendado)**
Se estiver usando VS Code:
1. Instale a extensão "Live Server"
2. Clique com botão direito no `portifolio.html`
3. Selecione "Open with Live Server"

## ✏️ Personalização

### Alterar Informações Pessoais

**No arquivo `portifolio.html`:**

1. **Nome e Título:**
```html
<h1>Aline Daiane Carneiro</h1>
<p class="subtitle">Seu novo título aqui</p>
```

2. **Email e Contatos:**
Busque por `aline@example.com` e `+55 (41)` e atualize com seus dados reais

3. **Links Sociais:**
```html
<a href="https://linkedin.com/in/seu-perfil" target="_blank">
```

4. **Cores Principais:**

No arquivo `style.css`, altere as variáveis:
```css
:root {
    --primary-color: #6366f1;        /* Cor principal */
    --secondary-color: #8b5cf6;      /* Cor secundária */
    --accent-color: #ec4899;         /* Cor de destaque */
}
```

### Adicionar Projetos

Crie uma nova seção no HTML:
```html
<section id="projetos" class="projetos">
    <div class="container">
        <h2>Meus Projetos</h2>
        <div class="projetos-grid">
            <!-- Adicione seus projetos aqui -->
        </div>
    </div>
</section>
```

## ⚡ Funcionalidades

### ✅ Implementadas
- [x] Navegação responsiva com hamburger menu
- [x] Hero section com call-to-action
- [x] Seção "Sobre" com estatísticas
- [x] Grid de competências
- [x] Timeline de experiência profissional
- [x] Cards de formação acadêmica
- [x] Formulário de contato funcional
- [x] Links sociais
- [x] Scroll suave
- [x] Animações ao carregamento
- [x] Footer informativo

### 🔜 Sugestões Futuras
- [ ] Adicionar seção de portfólio/projetos
- [ ] Integrar envio de emails (Formspree, EmailJS)
- [ ] Dark mode completo
- [ ] Blog ou artigos
- [ ] Certificados e badges
- [ ] Google Analytics

## 🌐 Deploy

### **GitHub Pages (Recomendado)**

1. Crie um repositório no GitHub chamado `portifolio_Aline`
2. Faça push de todos os arquivos
3. Vá em Settings → Pages
4. Selecione `main` branch como source
5. Seu site estará em: `https://seu-usuario.github.io/portifolio_Aline`

### **Netlify**

1. Conecte seu repositório GitHub
2. Configure build settings (deixe em branco para site estático)
3. Deploy automático!

### **Vercel**

1. Importe seu repositório
2. Clique em "Deploy"
3. Seu site estará ao vivo em minutos

## 📱 Responsividade

O portfólio é totalmente responsivo:

| Dispositivo | Breakpoint |
|-------------|-----------|
| Mobile | < 480px |
| Tablet | 480px - 768px |
| Desktop | > 768px |

## 📊 Otimizações

- ✅ Imagens otimizadas (lazy loading)
- ✅ CSS minificado (pode ser feito)
- ✅ JavaScript eficiente
- ✅ SEO friendly
- ✅ Acessibilidade (A11y)

## 🎨 Paleta de Cores

```
Primária:     #6366f1 (Indigo)
Secundária:   #8b5cf6 (Violeta)
Destaque:     #ec4899 (Rosa)
Escuro:       #1e293b (Cinza Escuro)
Claro:        #f8fafc (Cinza Claro)
```

## 📝 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🤝 Contribuições

Contribuições são bem-vindas! Para grandes mudanças, abra uma issue primeiro para discutir suas propostas.

## 📞 Contato

- **Email:** aline@example.com
- **LinkedIn:** [Aline Daiane Carneiro](https://linkedin.com/in/aline-daiane)
- **GitHub:** [seu-usuario](https://github.com)
- **Localização:** Curitiba, Paraná, Brasil

---

<div align="center">

### Desenvolvido com ❤️ por Aline Daiane Carneiro

⭐ Se gostou, considere dar uma estrela!

</div>
