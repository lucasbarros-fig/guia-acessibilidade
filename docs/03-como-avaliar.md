# 3. Como avaliar uma tela

A avaliação acontece no desenho, antes de a tela ir para o desenvolvimento. O método é o do [DA11Y.md](https://github.com/fecarrico/DA11Y.md), a edição de design do A11Y.md, no perfil **Standard (AA)**.

## Quando

- Toda tela nova ou alterada, antes de ser entregue.
- Nos dois modos de cor, claro e escuro, porque um mesmo token pode passar num e falhar no outro.
- Nas quatro larguras: Desktop L (1728), Desktop S (1366), Tablet (768) e Mobile (390).
- Todo componente novo do design system, em todos os estados (padrão, hover, foco, pressionado, selecionado, erro, desabilitado).

## O que medir

| O que | Como |
| --- | --- |
| Contraste | Fórmula da WCAG, com a cor do token resolvida no modo do frame. O texto é medido contra tudo o que está embaixo dele, e contra camadas semitransparentes por cima |
| Cor como único sinal | Ver a tela em escala de cinza e num simulador de daltonismo ([capítulo 5](05-daltonismo.md)) |
| Alvos | O frame do controle, nunca o ícone de dentro ([capítulo 8](08-alvos-de-toque.md)) |
| Estados | Cada controle tem foco desenhado, e os estados se distinguem sem depender só da cor |
| Intenção | O que o desenho não diz e o código vai precisar: nome de botão só com ícone, texto alternativo, ordem de leitura, anúncios |

Ficam isentos de contraste: componente desabilitado e logotipo.

## Severidade

| Severidade | O que significa | Exemplo |
| --- | --- | --- |
| Crítica | Impede a tarefa | Itens de menu sem estado de foco |
| Alta | Dificulta perceber ou ler | Texto branco num azul com 3,77:1; opção escolhida só pela cor |
| Média | Atrapalha ou fica abaixo de uma Regra da Casa | Alvo de 21 px; aviso que some em 3 s |
| Baixa | Polimento | Nome de camada que não diz o que é |

## Quem resolve

Cada achado tem um dono:

- **Decisão de quem desenha:** uma escolha que o desenho não resolve sozinho, como texto alternativo, nome de botão só com ícone, ou desabilitado versus somente leitura. Quem desenha decide a partir da proposta.
- **Corrigir no arquivo:** defeito de uso, como override, componente local ou peça feita à mão. Corrige-se no próprio arquivo.
- **Erro do design system:** defeito do componente ou do token. Corrige-se no design system, nunca por cima da instância, porque o mesmo defeito aparece em todas as telas que usam ele.

## Quem aprova

- Quem desenhou entrega como **autoavaliado**.
- Outra pessoa confere e só então a tela é **aprovada**.
- Uma exceção à norma é decisão da pessoa responsável pelo produto e fica registrada com dono, aprovador e prazo.

## Onde registrar

- O relatório da avaliação fica no repositório do produto, como um estudo de caso feito a partir do [modelo](../estudos-de-caso/_modelo.md).
- Anotações dentro do Figma só quando o time do arquivo pedir. O padrão é o relatório, para não poluir os protótipos.
- Corrigir é outro passo: a avaliação aponta e propõe; a mudança no arquivo ou no design system só acontece com a pessoa responsável de acordo.
