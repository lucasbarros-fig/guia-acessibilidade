# Como contribuir

O guia é do time inteiro. Qualquer pessoa pode propor uma mudança.

## Mudar ou criar uma regra

1. Abra um pull request com a mudança no capítulo certo, em `docs/`.
2. Toda regra cita de onde vem:
   - o critério da WCAG 2.2 e o item da ABNT NBR 17225, no formato `WCAG 1.4.1 · NBR 5.11.1`; ou
   - **Regra da Casa**, quando pedimos mais que a norma, com uma frase dizendo por quê.
3. Outra pessoa revisa. Ninguém aprova a própria mudança.
4. Registre a mudança no [CHANGELOG.md](CHANGELOG.md).

Se a mudança altera a página visual, atualize também `site/index.html`.

## Registrar um estudo de caso

1. No repositório do produto, crie uma pasta para o estudo, por exemplo `acessibilidade/estudo-2026-10/`.
2. Copie o [modelo](estudos-de-caso/_modelo.md) para `README.md` dentro dela e preencha.
3. Coloque os relatórios completos na mesma pasta.

Estudos de produtos internos não entram neste repositório, que é público: eles trazem dados do produto, links de arquivos e achados que não devem ficar abertos.

Um estudo descreve o que foi medido num produto. Ele não muda as regras gerais. Se o estudo mostrar que uma regra precisa mudar, abra um pull request separado para o capítulo.

## Como escrever

- Português do Brasil, frases curtas e voz ativa.
- Diga o que fazer, depois por quê. Um exemplo real vale mais que uma explicação longa.
- Números com vírgula decimal: `4,5:1`, `1,5 vez a fonte`.
- Nome de componente e de token como aparece no design system, entre crases: `Button`, `#166cba`.
- Sem “clique aqui”, sem emoji como marcador.

## Fontes e direitos

- Cite a fonte de todo dado e de toda prática que veio de fora. A lista fica em [docs/referencias.md](docs/referencias.md).
- Parafraseie. Citação literal só curta, entre aspas e com autoria.
- A ABNT NBR 17225 é protegida por direitos autorais da ABNT: cite o número e o nome do item, nunca copie o texto da norma.
