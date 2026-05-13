# 🚀 Guia de Deploy — GitHub Pages

## O que você vai ter no final
URL pública tipo: `https://seu-usuario.github.io/hospitalar2026/`  
Acesso por qualquer celular/computador, sem instalar nada.

---

## Passo a passo

### 1. Crie uma conta no GitHub (se ainda não tiver)
Acesse https://github.com e crie uma conta gratuita.

---

### 2. Crie um repositório novo

1. Clique no **+** no canto superior direito → **New repository**
2. Preencha:
   - **Repository name:** `hospitalar2026`
   - **Visibility:** ⚠️ Escolha com cuidado:
     - `Private` → só você vê (mas o GitHub Pages gratuito exige conta Pro)
     - `Public` → qualquer pessoa pode ver o código (mas o app fica online grátis)
3. **NÃO** marque "Add a README file"
4. Clique em **Create repository**

---

### 3. Suba os arquivos

**Opção A — pelo navegador (mais fácil):**
1. Na página do repositório recém-criado, clique em **uploading an existing file**
2. Arraste os arquivos `index.html`, `README.md` e `.gitignore` para a área de upload
3. Clique em **Commit changes**

**Opção B — pelo terminal (se tiver Git instalado):**
```bash
cd pasta-hospitalar2026
git init
git add .
git commit -m "Deploy inicial"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/hospitalar2026.git
git push -u origin main
```

---

### 4. Ative o GitHub Pages

1. No repositório, vá em **Settings** (engrenagem no topo)
2. No menu lateral, clique em **Pages**
3. Em **Source**, selecione:
   - Branch: `main`
   - Folder: `/ (root)`
4. Clique em **Save**
5. Aguarde ~1 minuto e atualize a página

Você verá uma mensagem:  
✅ *"Your site is live at https://seu-usuario.github.io/hospitalar2026/"*

---

### 5. Acesse o app

Abra a URL no celular ou computador.  
Compartilhe com a equipe de vendas!

---

## Para atualizar o app no futuro

1. Edite o `index.html` localmente
2. Acesse o repositório no GitHub
3. Clique no arquivo `index.html` → ícone de lápis ✏️ → cole o novo conteúdo → **Commit**
4. O site atualiza automaticamente em ~1 minuto

---

## ⚠️ Dicas importantes

- **Senhas e logins** ficam no `localStorage` do navegador de cada usuário — não são compartilhadas entre dispositivos. Cada pessoa faz seu próprio login na primeira vez.
- **JOLT (IA):** funciona abrindo o Claude.ai com o prompt pronto. O usuário precisa ter uma conta no Claude.ai (gratuita funciona).
- **Dados do pipeline** são locais no navegador. Se limpar o cache, os dados somem. Para dados persistentes compartilhados entre a equipe, considere uma versão futura com backend.
