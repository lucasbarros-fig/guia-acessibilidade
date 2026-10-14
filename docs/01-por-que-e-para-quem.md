# 1. Por que e para quem

> “O mundo já está na web e não podemos deixar ninguém de fora.”
> Joseana Mar e Gabriela Castro, UX Collective Brasil

## Acessibilidade como cultura

Romeu Sassaki, referência da inclusão social no Brasil, separa a acessibilidade em seis dimensões. Uma tela acessível resolve a dimensão comunicacional. Mas ela só continua acessível quando as outras também mudam: o jeito de trabalhar, as regras que adotamos e a atitude do time.

| Dimensão | Sem barreiras em… | Onde entra no nosso trabalho |
| --- | --- | --- |
| Comunicacional | escrita, fala, sinais e meio digital | As telas e os textos dos produtos |
| Metodológica | métodos e técnicas de trabalho e estudo | Avaliar antes de entregar ([capítulo 3](03-como-avaliar.md)) |
| Programática | normas, leis e políticas | WCAG, NBR 17225 e Lei Brasileira de Inclusão ([capítulo 2](02-normas.md)) |
| Atitudinal | preconceitos, estigmas e estereótipos | A cultura do time |
| Instrumental | instrumentos, utensílios e ferramentas | Design systems e ferramentas que já nascem acessíveis |
| Arquitetônica | espaços físicos | Fora do escopo deste guia |

Na prática, cultura aqui quer dizer três hábitos:

1. **Entra no desenho, não no fim.** Contraste, foco e textos são decididos junto com o layout, no Figma e no design system.
2. **Ninguém aprova o próprio desenho.** Quem desenhou entrega como autoavaliado e outra pessoa confere.
3. **Exceção tem dono.** Quando acessibilidade e identidade visual entram em conflito, quem decide é a pessoa responsável pelo produto. A exceção fica registrada com aprovador e prazo.

## Para quem desenhamos

A ABNT NBR 17225 fala em necessidades de acessibilidade situacionais, temporárias ou permanentes. Por isso a lista inclui a situação do momento: o que ajuda uma pessoa com deficiência ajuda todo mundo.

| Quem | O que acontece | O que ajuda | Capítulo |
| --- | --- | --- | --- |
| Pessoa daltônica | Não distingue certas cores. Atinge cerca de 1 em cada 12 homens e 1 em cada 200 mulheres | Cor sempre acompanhada de ícone, texto ou forma | [5](05-daltonismo.md) |
| Pessoa com dislexia | Decodificar o texto custa mais; algumas pessoas veem letras borradas ou que parecem se mexer | Texto à esquerda, curto, com bom espaçamento | [6](06-leitura-e-dislexia.md) |
| Pessoa com baixa visão | Precisa de contraste e de ampliar a tela sem perder conteúdo | 4,5:1 no texto e layout que acompanha o zoom sem rolagem lateral | [4](04-cor-e-contraste.md), [13](13-responsivo.md) |
| Quem usa só o teclado | Navega com Tab, setas e Enter, sem mouse | Foco visível em todo controle e ordem lógica | [7](07-foco-e-teclado.md) |
| Quem usa leitor de tela | Ouve a tela em vez de vê-la | Rótulos, nomes de botão e texto alternativo | [9](09-formularios.md), [10](10-componentes.md), [11](11-imagens-e-midia.md) |
| Quem tem tremor ou pouca precisão | Erra alvos pequenos e próximos | Alvos grandes e afastados | [8](08-alvos-de-toque.md) |
| Quem se distrai ou se cansa com movimento | Animação e prazos curtos atrapalham | Versão parada, nada que suma sozinho | [12](12-movimento-e-tempo.md) |
| Qualquer pessoa, num dado momento | Sol na tela, celular numa mão, pressa, internet lenta | Tudo o que está acima | todos |

## Por que vale a pena

- **É lei.** A Lei Brasileira de Inclusão obriga sites de empresas com sede ou representação no Brasil a serem acessíveis ([capítulo 2](02-normas.md)).
- **É mais gente usando.** Uma barreira tira do produto quem esbarra nela, e muitas vezes essa pessoa não volta.
- **É melhor para todos.** Contraste ajuda no sol, legenda ajuda sem som, texto curto ajuda com pressa.
- **Sai mais barato no começo.** Corrigir um token no design system resolve todas as telas que usam ele; corrigir depois de construído é tela por tela.
