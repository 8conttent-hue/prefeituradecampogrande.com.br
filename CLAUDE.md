# CLAUDE.md — PREFEITURADECAMPOGRANDE

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** PREFEITURADECAMPOGRANDE
**Nicho:** Casa e Decoração
**Keywords:** Ola Sou Regina Albuquerque Urbanista sociologa e professora da faculdade de arquitetura
**Paleta de cores:** teal | **Fonte:** lora

Olá! Sou Regina Albuquerque, Urbanista, socióloga e professora da faculdade de arquitetura e urbanismo da UFMS. Nascida e criada na cidade de Campo Grande, sou uma pessoa simples e humilde que tem o desejo de transmitir meu conhecimento através da internet. Atuando por mais de 7 anos na gestão de projetos na prefeitura de Campo Grande, Mato Grosso do Sul. Sou autora dos livros “A Cidade é para todos”, “Como viver na Cidade atual”. Publico constantemente notícias, artigos, conteúdos, relacionados ao urbanismo. Para você receber todo esse conteúdo direto no seu e-mail, basta se inscrever em minha newsletter.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-B |
| Hero | Hero-I |
| Features | Features-E |
| About Section | About-G |
| Posts | Posts-E |
| Footer | Footer-H |
| Página Sobre | Sobre-B |
| Página Contato | Contato-A |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
