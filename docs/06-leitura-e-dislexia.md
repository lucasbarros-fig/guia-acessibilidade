# 6. Leitura e dislexia

`WCAG 1.4.8, 1.4.12 e 3.1.5 · NBR 5.12`

A dislexia afeta a parte da leitura que transforma letras em palavras. Ler passa a pedir mais esforço, e algumas pessoas percebem o texto borrado, com letras que parecem trocar de lugar ou com “rios” de espaço branco cortando o parágrafo. Cada pessoa sente de um jeito, mas as mesmas escolhas de texto ajudam quase todas, e deixam a leitura mais fácil para todo mundo.

## Práticas

| Prática | Por quê | Norma |
| --- | --- | --- |
| Alinhar à esquerda, nunca justificar | O justificado abre espaços irregulares entre palavras, que se alinham em “rios” e puxam o olho para baixo | NBR 5.12.5 (recomendação) · WCAG 1.4.8 |
| Uma ideia por parágrafo | Pessoas com dislexia precisam de mais pausas entre os assuntos | Boa prática |
| Poucas palavras, as importantes primeiro | Menos texto para decodificar; a palavra-chave aparece logo | NBR 5.12.12 (recomendação) e ABNT NBR ISO 24495-1, linguagem simples |
| Fonte sem serifa no texto da interface | Sem os ganchos nas pontas, as letras ficam mais fáceis de separar | Boa prática |
| Caixa alta só em rótulo curto | Em maiúsculas todas as letras têm a mesma altura e a palavra perde o desenho | Boa prática |
| Texto corrido em 16 px | 16 px equivalem a 12 pt, dentro da faixa de 10 a 15 pt que o artigo do UX Collective indica. Corpo pequeno fica ilegível para quem tem dislexia ou baixa visão | Boa prática |
| Texto que amplia a 200% sem perder nada | Muita gente lê com zoom | WCAG 1.4.4 · NBR 5.12.7 (requisito) |
| Entrelinha de pelo menos 1,5 | Linhas apertadas se misturam | WCAG 1.4.12 · NBR 5.12.1 (requisito) |
| Até 80 caracteres por linha | Linha longa faz o olho se perder na volta | NBR 5.12.6 (requisito) |
| Espaçamento ajustável sem quebrar | Muita gente aumenta o espaço entre letras e linhas para conseguir ler | WCAG 1.4.12 · NBR 5.12.1 a 5.12.4 (requisitos) |

## O teste de espaçamento

A NBR e a WCAG usam estes valores de referência. O texto precisa continuar inteiro e funcionando quando eles são aplicados:

| Espaçamento | Valor |
| --- | --- |
| Entre linhas | 1,5 vez o tamanho da fonte |
| Entre parágrafos | 2 vezes o tamanho da fonte |
| Entre letras | 0,12 vez o tamanho da fonte |
| Entre palavras | 0,16 vez o tamanho da fonte |

No Figma, isso quer dizer **caixas de texto e contêineres com altura que cresce com o conteúdo (Hug)**, nunca altura fixa nem corte com reticências em texto que a pessoa precisa ler. A [página do guia](../site/index.html) tem um botão que aplica esses valores e mostra a diferença entre os dois casos.

## O que conferir no seu design system

- A entrelinha dos estilos de texto corrido: 1,5 ou mais.
- O tamanho do corpo de texto: 16 px para texto corrido; tamanhos menores só em rótulo e legenda curta.
- A família tipográfica da interface: sem serifa.
- Uma largura máxima para blocos de texto longo (termos, notícias, ajuda), em torno de 70 a 80 caracteres.
- Componentes que mostram texto sem altura fixa.
