# EDITS.md — Charme e Flores

> Arquivo de alterações pendentes e em progresso.
> Leia este arquivo junto ao CLAUDE.md antes de qualquer tarefa de edição.
> Marque cada item com [x] quando concluído.

---

## Edits Visuais

- [x] **Hero — espaçamento da logo e subtítulo**
  - Reduzir `margin-bottom` da logo para aproximá-la do texto "Charme e Flores"
  - Reduzir `margin-top` do texto "Charme e Flores" para ficar mais colado à logo
  - Reduzir distância entre o texto "Charme e Flores" e o subtítulo `.hero-script`
  - Resultado final: logo + título + subtítulo formam um bloco visual uniforme e premium
  - Não quebrar responsividade mobile

- [x] **Hero — botão Explorar (`.hero-scroll`)**
  - Adicionar `margin-top` leve no `.hero-scroll` para afastá-lo levemente dos botões acima
  - Não quebrar layout nem responsividade mobile

- [x] **Cards de produto — `.prod-img` prontos para imagem real**
  - Remover SVG placeholder e background gradiente de cada `.prod-img`
  - Substituir por tag `<img>` com `src` apontando para os respectivos arquivos:
    - Card 1 (Buquê Encantado): `media/products/buque.jpg`
    - Card 2 (Chaveiro Florzinha): `media/products/chaveiro.jpg`
    - Card 3 (Luminária Jardim Mágico): `media/products/luminaria.jpg`
  - Estilo da imagem: `width: 100%; height: 100%; object-fit: cover;`
  - Manter as dimensões e proporção do `.prod-img` atual
  - Enquanto a imagem não existir na pasta, exibir fundo rosa suave `#FDE8EE` como fallback