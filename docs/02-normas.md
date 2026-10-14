# 2. Normas: WCAG 2.2, ABNT NBR 17225 e a lei

O guia segue duas referências que dizem a mesma coisa, uma internacional e uma brasileira, e uma lei que torna a acessibilidade obrigatória.

## WCAG 2.2

As Diretrizes de Acessibilidade para Conteúdo Web, do W3C, são a referência internacional. Cada critério de sucesso tem um nível:

- **A:** o básico. Sem ele, muita gente fica de fora.
- **AA:** o nível recomendado para a maioria do conteúdo. **É o nosso mínimo.**
- **AAA:** o mais rígido. Não dá para exigir em todo conteúdo.

## ABNT NBR 17225:2025

*Acessibilidade em conteúdo e aplicações web — Requisitos* é a norma brasileira, publicada pela ABNT em 11 de março de 2025. Foi feita pela Comissão de Estudo de Acessibilidade para a Inclusão Digital (ABNT/CB-040), com o Ceweb.br e o NIC.br, e passou por consulta nacional no fim de 2024. Ela segue os critérios da WCAG 2.2, reescritos em português como itens numerados.

| Termo da NBR | O que quer dizer | Para nós |
| --- | --- | --- |
| Requisito | Item que precisa ser cumprido. Cobre os níveis A e AA da WCAG | Obrigatório |
| Recomendação | Nível AAA e boas práticas que não dá para exigir em todo contexto | Meta, não bloqueia a entrega |
| Conformidade regular | Todos os requisitos atendidos. Equivale à WCAG 2.2 AA | Nosso mínimo |
| Conformidade plena | Requisitos e recomendações. Recomendação que ficar de fora precisa de justificativa | Onde der |

Cada item da NBR diz qual critério da WCAG atende. Por isso o que medimos pela WCAG vale para a NBR, sem refazer a avaliação.

## A lei

Norma da ABNT é voluntária. Mas a **Lei Brasileira de Inclusão** (Lei 13.146/2015, art. 63) torna obrigatória a acessibilidade nos sites de empresas com sede ou representação no Brasil e de órgãos de governo, seguindo as diretrizes adotadas internacionalmente. A NBR 17225 foi escrita para atender essa lei. É a referência brasileira mais direta para mostrar que um produto cumpre o que a lei pede.

## Regra da Casa

Quando este guia pede mais que a norma, a regra é marcada como **Regra da Casa**. Exemplo: a WCAG pede alvos de 24 px; a Regra da Casa é 44 px. Uma Regra da Casa não cumprida não é falha de norma, mas vira um achado a resolver.

## O que a NBR deixa mais concreto para o design

Quase tudo coincide com a WCAG. Estes pontos merecem atenção porque a NBR dá números ou chama de requisito:

- **Espaçamento do texto (5.12.1 a 5.12.4, requisitos):** entrelinha de pelo menos 1,5 vez a fonte, parágrafos separados por 2 vezes, letras por 0,12 e palavras por 0,16, ou um jeito de configurar esse espaçamento sem cortar texto nem perder função. Veja [Leitura e dislexia](06-leitura-e-dislexia.md).
- **Largura do texto corrido (5.12.6, requisito):** até 80 caracteres por linha, ou um jeito de ajustar a largura.
- **Alvos (5.8.7, requisito; 5.8.6, recomendação):** 24 px é o mínimo; 44 px é a recomendação aprimorada, e a nossa Regra da Casa.
- **Foco (5.1.1 e 5.11.6, requisitos; 5.10.5, recomendação):** foco visível, com 3:1 contra o fundo e entre os estados. Um anel de 2 px por fora do controle cumpre também a recomendação.

## Mapa rápido WCAG × NBR

Os critérios que este guia mais usa. A coluna da NBR foi conferida no texto da norma.

| Assunto | WCAG 2.2 | Nível | NBR 17225 | Tipo na NBR |
| --- | --- | --- | --- | --- |
| Informação só pela cor | 1.4.1 | A | 5.11.1 Uso de cores | Requisito |
| Instrução só por cor, forma ou posição | 1.3.3 | A | 5.10.1 Características sensoriais | Requisito |
| Contraste de texto | 1.4.3 | AA | 5.11.3 Contraste para texto (mínimo) | Requisito |
| Contraste de texto, aprimorado | 1.4.6 | AAA | 5.11.2 Contraste para texto (aprimorado) | Recomendação |
| Contraste de componentes e gráficos | 1.4.11 | AA | 5.11.4 Componentes e 5.11.5 Objetos gráficos | Requisitos |
| Contraste do foco | 1.4.11 | AA | 5.11.6 Indicador de foco visível | Requisito |
| Foco visível | 2.4.7 | AA | 5.1.1 Indicador de foco visível | Requisito |
| Foco não escondido | 2.4.11 | AA | 5.1.3 Elemento em foco parcialmente visível | Requisito |
| Área do indicador de foco | 2.4.13 | AAA | 5.10.5 Área do indicador de foco visível | Recomendação |
| Alvo mínimo | 2.5.8 | AA | 5.8.7 Área de acionamento (mínima) | Requisito |
| Alvo aprimorado | 2.5.5 | AAA | 5.8.6 Área de acionamento (aprimorada) | Recomendação |
| Arrastar | 2.5.7 | AA | 5.8.13 Operação por movimento de arrastar | Requisito |
| Rótulo de campo | 3.3.2 e 4.1.2 | A | 5.9.1 Rótulo de campo | Requisito |
| Autenticação sem teste cognitivo | 3.3.8 | AA | 5.9.18 Autenticação acessível (mínima) | Requisito |
| Orientação | 1.3.4 | AA | 5.10.3 Orientação de exibição | Requisito |
| Conteúdo que se reorganiza com zoom, sem rolagem lateral | 1.4.10 | AA | 5.10.4 Design responsivo | Requisito |
| Texto ampliado a 200% | 1.4.4 | AA | 5.12.7 Texto redimensionado | Requisito |
| Espaçamento de texto | 1.4.12 | AA | 5.12.1 a 5.12.4 | Requisitos |
| Largura do texto | 1.4.10 e 1.4.8 | AA e AAA | 5.12.6 Largura de blocos de texto | Requisito |
| Alinhamento do texto | 1.4.8 | AAA | 5.12.5 Alinhamento de blocos de texto | Recomendação |
| Linguagem simples | 3.1.5 | AAA | 5.12.12 Nível de linguagem | Recomendação |

Para os demais critérios, o [Guia WCAG](http://guia-wcag.com/) mostra cada critério em português com o item correspondente da NBR.
