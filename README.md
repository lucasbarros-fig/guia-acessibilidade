# Guia de acessibilidade

Regras e práticas de acessibilidade para **todos os produtos e design systems** do time. Vale para quem desenha, quem desenvolve e quem decide o produto.

Toda tela precisa funcionar para quem não distingue cores, lê com dificuldade, enxerga pouco, usa só o teclado ou um leitor de tela, e também para quem está com o sol batendo na tela ou com uma mão ocupada. Se alguém não consegue terminar a tarefa por causa de uma barreira, a tela está quebrada, não quase pronta.

## Nível exigido

| Nível | O que é | Na entrega |
| --- | --- | --- |
| **WCAG 2.2 AA** = conformidade regular da **ABNT NBR 17225** | O mínimo legal e técnico | Obrigatório. Sem ele, a tela não é entregue |
| **Regra da Casa** | Onde este guia pede mais que a norma (exemplo: alvos de 44 px) | Esperado. Quando não cumprida, vira um achado a resolver |
| **WCAG AAA** = recomendações da NBR 17225 | Boas práticas mais rígidas | Meta. Não bloqueia a entrega |

## Por onde começar

| Você é | Comece por |
| --- | --- |
| Designer | [Cor e contraste](docs/04-cor-e-contraste.md) até [Responsivo](docs/13-responsivo.md), e o [checklist](docs/checklist.md) antes de entregar |
| Dev | [Foco e teclado](docs/07-foco-e-teclado.md), [Formulários](docs/09-formularios.md), [Componentes](docs/10-componentes.md), [Imagens e mídia](docs/11-imagens-e-midia.md) e [Movimento e tempo](docs/12-movimento-e-tempo.md) |
| Produto | [Por que e para quem](docs/01-por-que-e-para-quem.md), [Normas](docs/02-normas.md) e [Como avaliar](docs/03-como-avaliar.md) |
| Quem mantém um design system | [Cor e contraste](docs/04-cor-e-contraste.md), [Daltonismo](docs/05-daltonismo.md), [Foco e teclado](docs/07-foco-e-teclado.md), [Alvos de toque](docs/08-alvos-de-toque.md) |

## Capítulos

1. [Por que e para quem](docs/01-por-que-e-para-quem.md)
2. [Normas: WCAG 2.2, ABNT NBR 17225 e a lei](docs/02-normas.md)
3. [Como avaliar uma tela](docs/03-como-avaliar.md)
4. [Cor e contraste](docs/04-cor-e-contraste.md)
5. [Daltonismo](docs/05-daltonismo.md)
6. [Leitura e dislexia](docs/06-leitura-e-dislexia.md)
7. [Foco e teclado](docs/07-foco-e-teclado.md)
8. [Alvos de toque](docs/08-alvos-de-toque.md)
9. [Formulários](docs/09-formularios.md)
10. [Componentes e padrões](docs/10-componentes.md)
11. [Imagens e mídia](docs/11-imagens-e-midia.md)
12. [Movimento e tempo](docs/12-movimento-e-tempo.md)
13. [Responsivo](docs/13-responsivo.md)

Depois: o [checklist antes de entregar](docs/checklist.md) e as [referências](docs/referencias.md).

Cada regra traz o código da WCAG e o item da NBR 17225 que ela atende, por exemplo `WCAG 1.4.1 · NBR 5.11.1`.

## Estudos de caso

Os capítulos trazem a regra geral, que vale para qualquer produto. Um estudo de caso mostra a regra aplicada num produto real, com as medições daquele design system.

Os estudos ficam no repositório de cada produto, que costuma ser privado. Este repositório guarda só o [modelo](estudos-de-caso/_modelo.md) para registrar um.

## Página com exemplos

[`site/index.html`](site/index.html) é a versão visual do guia: exemplos “assim não / assim sim”, simulador de daltonismo, simulação de leitura e teste de espaçamento. Abra o arquivo no navegador.

## Como contribuir

Veja [CONTRIBUTING.md](CONTRIBUTING.md). Mudanças ficam registradas no [CHANGELOG.md](CHANGELOG.md).

## Créditos

O processo de avaliação usa o [DA11Y.md](https://github.com/fecarrico/DA11Y.md) e o [A11Y.md](https://github.com/fecarrico/A11Y.md), de Felipe A. Carriço, sob a licença MIT. Os capítulos de daltonismo e de leitura partem dos artigos de Joseana Mar e Gabriela Castro (UX Collective Brasil) e de Sojin Rank (AudioEye). A lista completa está nas [referências](docs/referencias.md).
