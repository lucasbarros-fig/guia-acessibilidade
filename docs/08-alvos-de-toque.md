# 8. Alvos de toque

`WCAG 2.5.8 e 2.5.5 · NBR 5.8.6 e 5.8.7`

O mínimo da WCAG e da NBR 17225 é **24 × 24 px**. A **Regra da Casa** é **44 × 44 px**, com **8 px** entre alvos vizinhos. Os 44 px coincidem com a recomendação aprimorada da NBR (5.8.6).

## Como medir

- **Meça o frame do controle**, nunca o ícone de dentro.
- Numa linha de checkbox ou radio, o rótulo clicável conta como parte do alvo.
- **Abaixo de 24 px** só passa pela exceção de espaçamento: um círculo de 24 px centrado no alvo não pode tocar outro alvo.
- **Abaixo de 44 px** não é falha de norma, mas é um achado a relatar.
- Link dentro de uma frase está isento do tamanho mínimo.

## O que conferir no seu design system

| Componente | O que verificar |
| --- | --- |
| Botões | Altura de 44 px ou mais |
| Botão só com ícone | Área clicável de 44 × 44, mesmo que o ícone seja de 20 |
| Variantes pequenas (small, bare, link) | Se ficam abaixo de 44, documente onde podem ser usadas e garanta o espaçamento |
| Checkbox, radio e switch | O rótulo faz parte do alvo |
| Itens de lista e de menu | Altura de 44 px ou mais |
