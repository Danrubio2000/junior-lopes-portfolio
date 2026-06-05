# CLAUDE.md - Junior Lopes Portfolio

## 📊 Visão Geral

**Junior Lopes - Artista Plástico Contemporâneo**

Landing page multilíngue (4 idiomas) para apresentar portfólio de obras de arte de Junior Lopes, artista plástico que trabalha com tecidos reciclados da indústria da moda.

**Status:** ✅ PRONTO E ONLINE

---

## 🎯 Objetivo do Projeto

Criar uma plataforma digital elegante e responsiva para:
- Apresentar o artista e sua história
- Exibir 15 obras de arte em alta resolução
- Listar exposições internacionais
- Destacar prêmios e reconhecimentos (Cannes, Taschen)
- Permitir contato direto (email, WhatsApp, telefone)

---

## 🌐 URLs Importantes

**Site Live:** https://danrubio2000.github.io/junior-lopes-portfolio/

**Repositório:** https://github.com/Danrubio2000/junior-lopes-portfolio

**Acesso Local (desenvolvimento):** http://localhost:8888/landing-page.html

---

## 📁 Estrutura do Projeto

```
junior-lopes-vercel/
├── landing-page.html          # Página principal (multilíngue)
├── index.html                 # Redirect para landing-page.html
├── images/
│   ├── IMAGENS/              # Fotos do artista e reconhecimentos
│   │   ├── Junior Lopes image.jpeg (foto principal)
│   │   ├── rolling stone 1.jpeg (reconhecimento)
│   │   ├── levis-11.jpeg
│   │   └── levis-12.jpeg
│   └── reorganized/          # Galeria de 15 obras
│       ├── obra_1.jpeg até obra_15.jpeg
│       └── obra_13.jpeg (Campanha Levi's - usada no hero)
├── apresentacao-v2.mp4       # Vídeo de apresentação
├── README.md                 # Documentação do projeto
└── .github/
    └── workflows/            # GitHub Actions (se necessário)
```

---

## 🎨 Features Implementadas

✅ **Multilíngue:** Português (PT), English (EN), Español (ES), Français (FR)
✅ **Responsivo:** Grid layouts, media queries para mobile
✅ **Hero Section:** Texto esquerda + Foto #11 direita (horizontais)
✅ **Sobre o Artista:** Texto + 2 imagens + 3 stats
✅ **Exposições:** 4 cards com info internacional
✅ **Prêmios:** 3 items + 2 imagens Levi's
✅ **Galeria:** 14 obras (obra_11 exclusiva no hero)
✅ **QR Code:** 1 único QR na navbar (landing page)
✅ **Language Switcher:** Botões PT/EN/ES/FR na navbar
✅ **Botão CTA:** "Explorar Obras" em amarelo (#FFD700)

---

## 🔧 Tecnologias

- **Frontend:** HTML5, CSS3, JavaScript vanilla
- **Biblioteca:** QRCode.js (CDN)
- **Deploy:** GitHub Pages (gh-pages branch)
- **Versionamento:** Git + GitHub

---

## 🎨 Design

- **Fundo:** Branco (#ffffff)
- **Borders:** Preto 1.5px (vinhetas finas)
- **Accents:** Amarelo #FFD700 (círculos, botões)
- **Tipografia:** Segoe UI, sans-serif
- **Layout:** CSS Grid + Flexbox

---

## 📐 Dimensões Importantes

| Elemento | Dimensão |
|----------|----------|
| Hero - Foto #11 | 100% × min-height 600px, object-fit: cover |
| Sobre - Foto Junior | 400px height |
| Sobre - Rolling Stone | 240px height, object-fit: contain |
| Galeria - Items | aspect-ratio: 1, object-fit: cover |
| QR Code - Navbar | 100×100px |

---

## 🌍 Multilingual Setup

Arquivo `landing-page.html` contém objeto `translations` com 4 languages:
- `translations.pt` → Português
- `translations.en` → English
- `translations.es` → Español
- `translations.fr` → Français

**Função:** `updateLanguage(lang)` atualiza toda página em tempo real.

---

## ⚠️ Lições Aprendidas

### GitHub Pages Issues Encontrados:
1. **Problema:** Workflow GitHub Actions falhava repetidamente
2. **Causa:** Token sem permissão `admin` para ativar Pages via API
3. **Solução:** Configuração manual via Settings → Pages → Source: gh-pages
4. **Resultado:** FUNCIONA! Não repita tentativas de API.

### Vercel/Netlify:
- Ambos começaram a cobrar (não usar para este projeto)
- GitHub Pages é a solução correta (gratuita para sempre)

### Imagens:
- GitHub Pages serve imagens corretamente via gh-pages branch
- Path relativo `images/reorganized/obra_11.jpeg` funciona

---

## 🚀 Como Continuar Desenvolvimento

### Para adicionar mudanças:
1. **Local:** Edita `landing-page.html`
2. **Teste:** Abre em `http://localhost:8888/landing-page.html`
3. **Commit:** `git add . && git commit -m "descrição"`
4. **Push:** `git push origin main`
5. **Live:** Automático em GitHub Pages (aguarda ~30 seg)

### Para adicionar novas linguagens:
1. Adiciona novo objeto em `translations.{lang}`
2. Adiciona botão na navbar `data-lang="{lang}"`
3. Adiciona event listener no JavaScript

### Para mudar imagens:
- Substitui em `/images/reorganized/` ou `/images/IMAGENS/`
- Atualiza src em HTML se necessário
- Push e aguarda deploy

---

## 📞 Contatos (conforme página)

- ✉️ Email: danielrubiodocs@gmail.com
- 📞 Telefone: +1 347-430-8188
- 💬 WhatsApp: +55 11 99449-4532

---

## ✅ Checklist Final

- [x] Site online e funcional
- [x] Todas as 15 obras carregando
- [x] 4 idiomas funcionando
- [x] QR code gerando corretamente
- [x] Imagens otimizadas
- [x] Responsivo (mobile/desktop)
- [x] GitHub Pages configurado
- [x] Repositório limpo (versão única)

---

## 📝 Notas para Próximas Sessões

**Importante:** Este projeto está PRONTO e PUBLICADO. Qualquer mudança é aprimoramento opcional.

**Não repita:**
- Tentativas de GitHub Actions workflow (use gh-pages direto)
- Vercel/Netlify (estão cobrando)
- Tentativas de API para ativar Pages (manual é necessário)

**Próximas mudanças planejadas:** Serão solicitadas pelo usuário na próxima sessão.

---

**Last Updated:** 2026-06-05
**Status:** PRODUCTION READY ✅
**Maintained by:** Daniel A. Rubio + Claude AI
