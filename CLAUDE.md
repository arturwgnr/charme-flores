# CLAUDE.md — Charme e Flores

> Guia de desenvolvimento para o site da Charme e Flores.
> Leia este arquivo antes de qualquer tarefa neste projeto.

---

## Sobre o Projeto

**Charme e Flores** é uma marca brasileira de flores artesanais (crochê/chenille), com estética kawaii/fofa e mascote coelhinho. O site é uma **vitrine premium com assistente de IA integrada**, sem carrinho de compras — o objetivo é encantar o visitante e direcionar para WhatsApp/Instagram para fechar pedidos.

---

## Skills Disponíveis

Antes de qualquer tarefa de frontend, consulte as skills em:

```
C:\Users\User\.claude\skills
```

Em especial:
- **frontend-design** — obrigatório para qualquer componente visual. Leia o SKILL.md antes de codar.
- Outras skills relevantes conforme a tarefa (ex: pdf, docx, xlsx se necessário).

---

## Stack

- **HTML + CSS + Vanilla JS** em arquivo único (sem framework)
- **Anthropic API** (`claude-sonnet-4-20250514`) para o chat da assistente IA
- **Sem backend** — estático, hospedável em qualquer CDN (Vercel, Netlify, GitHub Pages)
- **Sem dependências de build** — tudo via CDN se necessário

---

## Identidade Visual

### Paleta de Cores
```css
--color-primary:     #F4A7B9;   /* Rosa suave principal */
--color-primary-deep:#E8849A;   /* Rosa mais saturado */
--color-gold:        #D4AF7A;   /* Dourado premium (acentos) */
--color-gold-light:  #F0D9B0;   /* Dourado claro */
--color-white:       #FFFAF9;   /* Branco quente */
--color-text:        #3D2B2B;   /* Marrom escuro suave para texto */
--color-bg:          #FFF5F7;   /* Fundo levíssimo rosado */
```

### Tipografia
- **Títulos**: fonte script elegante (ex: `Playfair Display`, `Cormorant Garamond`, `Dancing Script` — escolher no contexto)
- **Corpo**: sans-serif refinada (ex: `DM Sans`, `Jost`, `Nunito`)
- **Nunca usar**: Inter, Roboto, Arial, system fonts genéricas

### Tom Visual
- Kawaii mas premium — não infantil
- Micro-animações suaves (pétalas caindo, hover delicado, fadeins)
- Espaço negativo generoso
- Dourado apenas como acento — não exagerar

---

## Estrutura do Site

```
/
├── Hero              — Logo, tagline, animação, CTA
├── Sobre             — História da marca
├── Categorias        — Cards expansíveis por categoria (genérico por enquanto)
├── Destaques         — Produtos em evidência
└── [Assistente IA]   — Chat flutuante sempre visível
```

### Categorias (genéricas por enquanto)
- Vasinhos Decorativos
- Chaveiros
- Luminárias & Porta-Retratos
- *(expandir conforme o cliente confirmar)*

---

## Assistente IA — Lua 🐰

### Identidade
- **Nome**: Lua
- **Personalidade**: fofa, acolhedora, profissional — fala como alguém da marca
- **Visual**: coelhinho mascote flutuante (SVG ou imagem), expressões dinâmicas

### Comportamento
- Responde dúvidas sobre produtos, prazos, preços, personalizações
- Sempre encerra com CTA direcionando para WhatsApp ou Instagram
- Tom: caloroso, nunca robótico

### Integração API
```javascript
const response = await fetch("https://api.anthropic.com/v1/messages", {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({
    model: "claude-sonnet-4-20250514",
    max_tokens: 1000,
    system: `Você é Lua, a assistente fofa da Charme e Flores 🐰
Fale de forma calorosa, use emojis com moderação, seja prestativa.
A loja vende flores artesanais de crochê/chenille: vasinhos, chaveiros, luminárias.
Sempre encerre sugerindo contato via WhatsApp ou Instagram para fazer um pedido.
Nunca invente preços específicos — diga que os valores variam e convide para conversar.`,
    messages: conversationHistory
  })
});
```

---

## Convenções de Código

- **Nomenclatura de arquivos**: `YYYY-MM-DD-descricao.html`
- **CSS**: variáveis globais no `:root`, mobile-first
- **JS**: sem frameworks, ES6+ moderno
- **Comentários**: em português, seções bem marcadas
- **Acessibilidade**: `alt` em imagens, contraste adequado, foco visível

---

## Regras de Desenvolvimento

1. **Sempre leia a skill `frontend-design`** antes de criar qualquer componente visual
2. **Proponha o plano primeiro** — não execute sem aprovação em tarefas multi-passo
3. **Confirme antes de sobrescrever** qualquer arquivo existente
4. **Liste arquivos criados/modificados** ao final de cada tarefa
5. **Mobile-first** — o público acessa majoritariamente pelo celular

---

## Contatos da Marca (preencher)

```
WhatsApp:  +55 (xx) xxxxx-xxxx
Instagram: @charme_e_flores
```

---

## Status do Projeto

- [x] Briefing e identidade visual definidos
- [ ] Arquivo HTML principal criado
- [ ] Hero section
- [ ] Seção Sobre
- [ ] Seção Categorias
- [ ] Seção Destaques
- [ ] Assistente IA (Lua) integrada
- [ ] Revisão mobile
- [ ] Deploy