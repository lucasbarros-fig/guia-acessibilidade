# 13. Responsivo

`WCAG 1.4.10, 1.4.4, 1.4.12 e 1.3.4 · NBR 5.10.3, 5.10.4, 5.12.6 e 5.12.7`

Desenhamos nas nossas quatro larguras. Não desenhamos 320 px.

| Página no Figma | Largura × altura |
| --- | --- |
| Desktop L | 1728 × 972 |
| Desktop S | 1366 × 769 |
| Tablet | 768 × 1024 |
| Mobile | 390 × 844 |

## Regras

- **Layout fluido:** o Mobile de 390 é desenhado com auto layout que estica e encolhe, sem nada com largura fixa maior que a tela. É isso que deixa o produto funcionar com zoom e em celulares menores sem rolagem lateral, o que a WCAG 1.4.10 e a NBR 5.10.4 conferem no produto construído.
- **Nada mais largo que a tela:** ações empilham, mensagens quebram linha, tabelas rolam dentro do próprio contêiner.
- **Texto que cresce:** texto que a pessoa lê não tem altura fixa nem corte com reticências. Ele precisa sobreviver a 200% e a espaçamento de texto maior ([capítulo 6](06-leitura-e-dislexia.md)).
- **Auto layout coerente:** um contêiner que se ajusta ao conteúdo (Hug) com um filho que preenche (Fill) se anula, e o filho encolhe até quase sumir.
- **Orientação:** retrato e paisagem, sem travar. `NBR 5.10.3`

## Para quem desenvolve

O layout fluido do desenho vira teste no código: com zoom de 400% num notebook (equivale a 320 px de largura), nada some e não aparece rolagem lateral.
