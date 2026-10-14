# 5. Daltonismo

`WCAG 1.4.1 · NBR 5.11.1`

**A cor nunca trabalha sozinha.** Para quem tem daltonismo, uma informação passada só pela cor desaparece. Mesmo com bom contraste entre duas cores, é preciso um sinal a mais: forma, ícone, texto ou sublinhado.

Cerca de 1 em cada 12 homens e 1 em cada 200 mulheres têm alguma deficiência na visão de cores. O tipo vermelho-verde é o mais comum.

## Os tipos

| Tipo | Como a pessoa enxerga | Frequência |
| --- | --- | --- |
| Deuteranomalia | Alguns verdes parecem mais vermelhos; forma leve | O tipo mais comum |
| Protanomalia | Alguns vermelhos parecem mais verdes e menos vivos; forma leve | Comum (vermelho-verde) |
| Protanopia e deuteranopia | Não diferenciam vermelho de verde | Comum (vermelho-verde) |
| Tritanomalia | Dificuldade entre azul e verde, e entre amarelo e vermelho | Menos comum (azul-amarelo) |
| Tritanopia | Não diferencia azul de verde, roxo de vermelho, amarelo de rosa; cores menos vivas | Menos comum (azul-amarelo) |
| Acromatopsia | Não vê cores, só tons de cinza | Rara |

Fonte: National Eye Institute.

## O que a WCAG e a NBR exigem

Nenhuma das duas cita tipos de daltonismo nem manda usar simulador: elas cobram o resultado.

| Critério WCAG 2.2 | Nível | Item da NBR 17225 | O que exige |
| --- | --- | --- | --- |
| 1.4.1 Uso de cor | A | 5.11.1 Uso de cores (requisito) | Nada transmite informação, indica ação, pede resposta ou destaca um elemento só pela cor |
| 1.3.3 Características sensoriais | A | 5.10.1 Características sensoriais (requisito); 5.8.15 Controles com retorno (recomendação) | Instrução não depende só de cor, forma, tamanho, posição ou som: “toque no botão verde” não basta |
| 1.4.3 Contraste (mínimo) | AA | 5.11.3 Contraste para texto, mínimo (requisito) | Texto 4,5:1; texto grande 3:1 |
| 1.4.11 Contraste não textual | AA | 5.11.4, 5.11.5 e 5.11.6 (requisitos) | 3:1 em bordas, ícones, partes de gráfico e foco |
| 1.4.6 Contraste (melhorado) | AAA | 5.11.2 Contraste para texto, aprimorado (recomendação) | Texto 7:1; texto grande 4,5:1 |

Os quatro primeiros são obrigatórios. O último é meta.

## Uma solução para todas as visões

Não é preciso uma adaptação para cada tipo. Se toda informação tem um sinal que não é cor e a tela continua legível em escala de cinza, ela funciona para a visão típica e para todos os tipos de daltonismo.

1. **Sinal duplo:** a cor reforça, mas quem explica é a forma, o ícone, a palavra, o sublinhado ou o peso.
2. **Funciona em cinza:** a escala de cinza é o caso mais rigoroso. Se a diferença aparece sem cor, aparece para todos.
3. **Claridade separa estados:** quando dois estados só podem mudar de cor, a diferença de claridade entre eles fica em 3:1 ou mais. Abaixo disso, entra a forma.
4. **Contraste mínimo:** texto 4,5:1 e ícone, borda e foco 3:1, no claro e no escuro.

## Práticas

| Prática | Como fazer | Fonte |
| --- | --- | --- |
| Rótulo junto da cor | Status, campo obrigatório e legenda levam palavra ou ícone além da cor | AudioEye (práticas 1, 2 e 4); UX Collective |
| Instrução pelo nome | “Toque em Continuar”, nunca “toque no botão verde” | UX Collective |
| Link parece link | Link dentro de texto é sempre sublinhado. Destaque usa peso ou tamanho | UX Collective; AudioEye (prática 5) |
| Linhas e marcas grossas | Prefira traços e sublinhados visíveis a filetes finos de cor | AudioEye (prática 5) |
| Textura em gráfico | Cada série tem textura, marcador ou tracejado e o nome escrito no próprio gráfico | AudioEye (prática 3) |
| Claridade, não só matiz | Varie claro e escuro, não só a cor. Confira em escala de cinza | AudioEye (prática 6) |
| Fuja das combinações de risco | Veja a lista abaixo | AudioEye (prática 7) |
| Paleta enxuta | Poucas cores, com variação de claridade | AudioEye (prática 8) |

### Combinações para evitar

Estes pares se confundem para muita gente. Se precisar usar algum, acrescente rótulo ou ícone.

- verde e vermelho
- verde e marrom
- verde e cinza
- verde e azul
- verde e preto
- verde-claro e amarelo
- azul e roxo
- azul e cinza

Para separar duas séries, prefira azul e laranja, uma clara e uma escura, com rótulo direto.

## Padrões de componente

| Situação | Como fazer |
| --- | --- |
| Opção escolhida (grupo de opções, filtros, cards selecionáveis) | Borda de 2 px, ícone de check e texto em negrito |
| Link dentro de texto | Sublinhado sempre |
| Posição num carrossel | Indicador atual com outra forma (mais largo) e “2 de 4” escrito |
| Erro de campo | Ícone, texto e cor |
| Status de um item | Texto ao lado do ponto colorido (“Documentos pendentes”) |
| Mensagens (toasts, alertas) | Rótulo escrito e ícone (“Sucesso”, “Informação”) |
| Critérios de senha | Ícone de check ou de x além da cor |
| Gráficos | Rótulo direto, textura ou tracejado em cada série, e 3:1 entre séries vizinhas |

## Como testar antes de entregar

1. Veja a tela em escala de cinza. Se uma informação some, ela depende só da cor.
2. Rode um simulador. No Figma, o plugin Stark. No Chrome, DevTools › Rendering › Emulate vision deficiencies.
3. Trate a simulação como aproximação e, sempre que der, valide com pessoas daltônicas.

A [página do guia](../site/index.html) tem um simulador com os mesmos filtros do Chrome aplicado a exemplos reais.

## Exemplos medidos

- Um verde `#1f7a4d` e um vermelho `#c0372b` de status têm 1,03:1 de claridade entre si. Em escala de cinza, “aprovado” e “recusado” viram a mesma cor: o status precisa de texto ou ícone.
- Um azul de link `#166cba` tem só 1,91:1 contra um texto `#374151`. Abaixo de 3:1, a cor não separa o link do texto em volta: o link precisa de sublinhado.
