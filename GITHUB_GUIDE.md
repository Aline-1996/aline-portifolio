# 📖 Guia Completo - Publicar no GitHub

## Passo 1: Preparar seu Repositório Local

### 1.1 Inicializar Git (se ainda não fez)
```bash
cd c:\xampp\htdocs\programadorweb\portifolio_Aline
git init
```

### 1.2 Adicionar todos os arquivos
```bash
git add .
```

### 1.3 Fazer o primeiro commit
```bash
git commit -m "feat: portfólio profissional inicial"
```

## Passo 2: Criar Repositório no GitHub

1. Acesse [github.com](https://github.com)
2. Clique em **"+"** → **"New repository"**
3. Preencha as informações:
   - **Repository name:** `portifolio` ou `aline-portifolio`
   - **Description:** "Portfólio profissional - Aline Daiane Carneiro"
   - **Público ou Privado:** Deixe públic
   - **Initialize with:** NÃO marque nada
4. Clique em **"Create repository"**

## Passo 3: Conectar e Fazer Push

### 3.1 Adicionar remote origin
```bash
git remote add origin https://github.com/seu-usuario/portifolio.git
```

### 3.2 Renomear branch (se necessário)
```bash
git branch -M main
```

### 3.3 Fazer push do código
```bash
git push -u origin main
```

## Passo 4: Ativar GitHub Pages

1. Vá até seu repositório no GitHub
2. Clique em **Settings** (engrenagem)
3. No menu esquerdo, clique em **Pages**
4. Em **Source**, selecione:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
5. Clique em **Save**

**Seu site estará disponível em:**
```
https://seu-usuario.github.io/portifolio
```

## Passo 5: Personalizar seu Portfólio

### Atualizar Links e Informações

**No arquivo `portifolio.html`:**

1. **Adicione seu Email Real:**
   ```html
   <a href="mailto:seu-email@example.com">seu-email@example.com</a>
   ```

2. **Atualize seu LinkedIn:**
   ```html
   <a href="https://linkedin.com/in/seu-usuario" target="_blank">
   ```

3. **Atualize seu GitHub:**
   ```html
   <a href="https://github.com/seu-usuario" target="_blank">
   ```

### Alterar Cores (Optional)

No `style.css`, modifique:
```css
:root {
    --primary-color: #6366f1;      /* Sua cor principal */
    --secondary-color: #8b5cf6;
    --accent-color: #ec4899;
}
```

## Passo 6: Fazer Commits Futuros

Quando fizer alterações:

```bash
# Ver alterações
git status

# Adicionar alterações
git add .

# Fazer commit com mensagem descritiva
git commit -m "fix: atualize email e redes sociais"

# Enviar para GitHub
git push origin main
```

## 📝 Mensagens de Commit Boas

```bash
feat: adicionar seção de projetos
fix: corrigir responsividade mobile
docs: atualizar README
style: melhorar paleta de cores
refactor: otimizar CSS
perf: lazy loading de imagens
test: adicionar testes
chore: atualizar dependências
```

## 🔗 URLs Úteis Após Deploy

- **Site ao vivo:** `https://seu-usuario.github.io/portifolio`
- **Repositório:** `https://github.com/seu-usuario/portifolio`
- **Editar:** Clone localmente e faça push novamente

## ⚠️ Troubleshooting

### Site não aparece após push
- Aguarde 5-10 minutos
- Limpe o cache do navegador (Ctrl+Shift+R)
- Verifique se GitHub Pages está ativado em Settings

### Erro de autenticação
```bash
# Gerar novo token: https://github.com/settings/tokens
# Use em vez de senha ao fazer push
```

### Mudar URL do repositório
```bash
git remote set-url origin https://github.com/novo-usuario/novo-repo.git
```

## 📊 Checklist Final

- [ ] Repositório criado no GitHub
- [ ] Código feito push para `main`
- [ ] GitHub Pages ativado
- [ ] Email atualizado no portfólio
- [ ] Links sociais corretos
- [ ] Site está acessível online
- [ ] README está bem formatado
- [ ] Arquivo `.gitignore` está presente

## 🎯 Próximos Passos

1. **Integrar formulário de contato:**
   - Use [Formspree](https://formspree.io/) ou [EmailJS](https://www.emailjs.com/)

2. **Adicionar projetos:**
   - Crie repositórios para seus projetos de programação
   - Linkue no portfólio

3. **Melhorar SEO:**
   - Adicione meta tags
   - Otimize imagens

4. **Analytics:**
   - Integre Google Analytics

5. **Certificados:**
   - Adicione uma seção de certificações

---

**Dúvidas?** Consulte a [documentação do GitHub Pages](https://docs.github.com/pt/pages)
