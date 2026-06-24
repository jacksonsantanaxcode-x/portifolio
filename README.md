# Portfólio Pessoal

Site de portfólio pessoal feito com HTML e CSS puro. Tema escuro, responsivo e com animações suaves.

## Estrutura de arquivos

```
portfolio/
├── index.html   → página principal
├── style.css    → todos os estilos
├── foto.jpg     → sua foto de perfil (adicione aqui)
├── cv.pdf       → seu currículo para download (adicione aqui)
└── README.md    → este arquivo
```

---

## O que substituir para personalizar

### 1. Seus dados pessoais (`index.html`)

| Onde encontrar | Substituir por |
|---|---|
| `Seu Nome` | seu nome completo |
| `SN` (iniciais do avatar) | suas iniciais reais |
| `Desenvolvedor IA & Automação` | seu cargo/especialidade |
| Texto da bio no hero | sua frase de apresentação |
| Texto da seção "Sobre mim" | sua história real |

### 2. Números das estatísticas (`index.html`)

Encontre a seção `id="sobre"` e edite:
- `12+` → quantidade de projetos que você fez
- `3+`  → seus anos de estudo/experiência
- `15+` → quantas tecnologias você usa
- `∞`   → o que quiser celebrar

### 3. Skills (`index.html`)

Encontre a seção `id="skills"` e:
- Adicione ou remova `<span class="tag">NomeDaTecnologia</span>`
- Renomeie os grupos (Frontend, Backend, Automação) se preferir outros

### 4. Projetos (`index.html`)

Para cada `<article class="project-card">`, edite:
- O emoji do ícone (`🤖`, `📊`, etc.)
- O título `project-card__title`
- A descrição `project-card__desc`
- As tags de tecnologia
- Os links do GitHub e Demo (atributo `href="#"`)

### 5. Contato (`index.html`)

Substitua nos três `<a class="contact-card">`:
- `seu@email.com` → seu e-mail real
- `github.com/seuusuario` → seu usuário do GitHub (duas ocorrências por card)
- `linkedin.com/in/seuusuario` → seu LinkedIn

### 6. Logo e rodapé

- `.nav__logo` no header: troque `SN` pelas suas iniciais
- `.footer__copy`: troque `Seu Nome` pelo seu nome

### 7. Meta tags (`<head>`)

- `<title>` → seu nome e cargo
- `<meta name="description">` → sua descrição curta

---

## Adicionar sua foto

Coloque sua foto na pasta com o nome **`foto.jpg`**.

- Formato recomendado: JPG ou PNG quadrado (ex: 400×400 px)
- Se não existir o arquivo, o site mostra suas iniciais automaticamente com fundo gradiente roxo

---

## Publicar no GitHub Pages (gratuito)

```bash
git init
git add .
git commit -m "meu portfolio"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/portfolio.git
git push -u origin main
```

Depois acesse o repositório → **Settings → Pages → Source: Deploy from branch → main** → Salvar.

Seu site ficará disponível em: `https://SEU-USUARIO.github.io/portfolio`

---

## Personalizar cores

Abra `style.css` e edite as variáveis no início do arquivo:

```css
:root {
  --accent: #7c5cfc;   /* cor roxa — troque pelo hex da sua cor favorita */
  --bg:     #0a0a0a;   /* fundo principal */
}
```

---

## Melhorias com Claude Code

Com o Claude Code aberto nesta pasta, você pode pedir:

- `"Adiciona animação de digitação no meu cargo"`
- `"Cria uma seção de linha do tempo com minha trajetória"`
- `"Adiciona um toggle de tema claro/escuro"`
- `"Coloca um contador animado nos números de estatísticas"`
- `"Adiciona partículas no fundo do hero"`
