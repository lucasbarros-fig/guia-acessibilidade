# 4. Cor e contraste

`WCAG 1.4.3, 1.4.11 e 1.4.6 · NBR 5.11.2 a 5.11.6`

Texto pequeno precisa de 4,5:1 contra o fundo; ícones, bordas e foco precisam de 3:1. Meça sempre no claro e no escuro.

## Os mínimos

| O que | Mínimo | Norma |
| --- | --- | --- |
| Texto até 23 px (ou até 18 px em negrito) | 4,5:1 | WCAG 1.4.3 · NBR 5.11.3 |
| Texto grande: 24 px, ou 18,66 px em negrito | 3:1 | WCAG 1.4.3 · NBR 5.11.3 |
| Ícone que informa, borda de controle, partes de gráfico | 3:1 | WCAG 1.4.11 · NBR 5.11.4 e 5.11.5 |
| Anel de foco, contra o fundo e entre os estados | 3:1 | WCAG 1.4.11 · NBR 5.11.6 |
| Componente desabilitado e logotipo | isento | WCAG 1.4.3 e 1.4.11 · NBR 5.11.3 e 5.11.4 |
| Meta para texto (AAA) | 7:1, ou 4,5:1 no texto grande | WCAG 1.4.6 · NBR 5.11.2 |

As medidas em px partem de 1 pt = 1,333 px: 18 pt = 24 px e 14 pt em negrito = 18,66 px.

## Como medir

- Use a fórmula da WCAG sobre a cor que aparece na tela: o token resolvido no modo do frame, com as camadas semitransparentes somadas ao fundo.
- Meça o par real. Texto sobre imagem ou gradiente é medido no pior ponto.
- No Figma, a checagem de contraste do seletor de cor serve para conferir. Não use o botão de correção automática: ele troca a cor da instância e fura o token.
- Confira os dois modos. Um token pode passar no claro e reprovar no escuro, ou o contrário.

## A cor da marca fica

A acessibilidade não pede para trocar a cor da marca. Ela pede para cada cor trabalhar onde passa:

- **Com 3:1 ou mais contra o fundo:** a cor serve para logotipo, ícones, bordas, seleção, barras e títulos grandes.
- **Para texto pequeno e links:** use um tom mais escuro que a própria paleta já tem, geralmente o de hover ou o de pressionado. Procure um tom existente antes de criar uma cor nova.
- **Botão com texto branco sobre a cor da marca abaixo de 4,5:1:** há três caminhos, e a escolha é de quem responde pelo produto.
  1. Usar o tom mais escuro da paleta como fundo do botão.
  2. Manter a cor e usar rótulo de texto grande (por exemplo, 19 px em negrito, que conta como texto grande).
  3. Manter e registrar a exceção, com aprovador e prazo.

## O que conferir no seu design system

- Cada par texto × fundo dos tokens semânticos, nos dois modos.
- Os tokens de feedback (sucesso, aviso, erro, informação) com o texto que vai por cima deles.
- O token de foco contra os fundos mais usados ([capítulo 7](07-foco-e-teclado.md)).
- Cores de status entre si: se dois estados só mudam de cor, a diferença de claridade entre eles precisa ser de 3:1 ou mais ([capítulo 5](05-daltonismo.md)).

## Exemplo

Um azul de marca `#2b87d9` tem 3,77:1 com o branco: serve para ícone, borda e seleção, mas não para texto pequeno. O tom de hover da mesma paleta, `#166cba`, tem 5,4:1 e resolve texto e links sem trocar a cor da marca.
