# EDITS.md — Charme e Flores

> Arquivo de alterações pendentes e em progresso.
> Leia este arquivo junto ao CLAUDE.md antes de qualquer tarefa de edição.
> Marque cada item com [x] quando concluído.

---

## Edits Visuais

- [x] **Hero — `.hero-blob-2` no mobile**
  - Apenas em telas mobile (`max-width: 768px`)
  - Reduzir tamanho: de `260px` para aproximadamente `140px`
  - Reposicionar para o canto superior direito (longe da logo)
  - Sugestão: `top: -30px; right: -40px; left: auto; bottom: auto;`
  - Não alterar comportamento no desktop

---

## Edits de Conteúdo

- [x] **WhatsApp — mensagens personalizadas por botão**
  - Atualizar o parâmetro `?text=` de cada link `wa.me` conforme abaixo
  - Todos os links devem manter o número `553191078401`

  | Botão | Mensagem (encode para URL) |
  |---|---|
  | Nav — "Pedir agora" | `Olá! Vim pelo site e gostaria de fazer um pedido 🌸` |
  | Hero — "Pedir pelo WhatsApp" | `Olá! Vim pelo site da Charme e Flores e gostaria de saber mais sobre as peças 🐰✨` |
  | Footer — "Fazer pedido" | `Olá! Cheguei até o fim do site e adorei tudo! Gostaria de fazer um pedido 🌸` |
  | Card — Buquê Encantado | `Olá! Vi o Buquê Encantado no site e me interessei 💐 Pode me contar mais?` |
  | Card — Chaveiro Florzinha | `Olá! Vi o Chaveiro Florzinha no site e adorei! 🌸 Gostaria de saber mais` |
  | Card — Luminária Jardim Mágico | `Olá! Vi a Luminária Jardim Mágico no site e fiquei encantada ✨ Pode me contar mais?` |
  | Footer social pill — WhatsApp | `Olá! Vim pelo site da Charme e Flores 🐰 Gostaria de conversar!` |