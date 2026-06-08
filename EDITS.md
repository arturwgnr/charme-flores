# EDITS.md — Charme e Flores

> Arquivo de alterações pendentes e em progresso.
> Leia este arquivo junto ao CLAUDE.md antes de qualquer tarefa de edição.
> Marque cada item com [x] quando concluído.

---

## Edits Gerais

- [ ] Substituir logo placeholder pela imagem real (`assets/logo.png`)
- [ ] Configurar API key da Anthropic no projeto

---

## Edits Claude (Assistente IA)

*(sem pendências no momento)*

---

## Edits Visuais

- [x] **Pétalas — comportamento em loop**
- [x] **Flor da seção Sobre** — rotação reduzida
- [x] **Hover nos elementos** — transição 0.6s aplicada

- [x] **Pétalas — z-index global (efeito premium)**
  - A queda de pétalas deve ser **contínua** (sem pausa)
  - As pétalas devem passar **atrás de todos os elementos** da página: footer, cards, botões, seções, navbar
  - Implementar via z-index baixo nas pétalas (ex: `z-index: 0`) e garantir que todos os elementos interativos e visuais tenham `z-index` explicitamente acima (ex: `position: relative; z-index: 1` nos cards, botões, footer, navbar)
  - O efeito deve dar sensação de profundidade — pétalas no plano de fundo, conteúdo no primeiro plano