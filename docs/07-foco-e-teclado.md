# 7. Foco e teclado

`WCAG 2.1.1, 2.4.3, 2.4.7, 2.4.11 e 1.4.11 · NBR 5.1 e 5.11.6`

Todo controle precisa de um estado de foco desenhado, porque quem usa o teclado só sabe onde está por ele.

## Regras

- **Anel de foco:** contorno de 2 px, com 3:1 contra o fundo, por fora do controle e com 2 px de folga. Por dentro de um botão colorido, o anel encosta na cor do botão e some. Nunca só sombra nem só troca de preenchimento. `NBR 5.1.1, 5.11.6 e 5.10.5`
- **Nunca escondido:** o controle com foco não pode ficar por baixo de um cabeçalho fixo, de um menu lateral ou de uma barra de ações fixa. `WCAG 2.4.11 · NBR 5.1.3`
- **Tudo pelo teclado:** toda ação feita com mouse ou toque também funciona com teclado. `WCAG 2.1.1`
- **Nada só por hover:** toda ação tem clique ou toque e um controle visível. Tooltip aparece também no foco.
- **Sem armadilha:** o foco sempre consegue sair de um componente. `NBR 5.1.6`
- **Ordem de leitura:** segue a ordem visual, que no Figma é a ordem do auto layout. Quando a ordem visual for outra, anote a ordem certa para quem desenvolve. `WCAG 2.4.3 · NBR 5.1.4`

## Teclado por componente

| Componente | Teclado |
| --- | --- |
| Menu suspenso (dropdown) | ↑ e ↓ entre os itens; Esc fecha e devolve o foco ao botão que abriu |
| Abas | ← e → entre as abas; Tab entra no painel |
| Grupo de opções (radio, cards selecionáveis) | Uma parada de Tab no grupo; ← e → trocam a opção |
| Diálogo e menu em gaveta | O foco vai para o título; Tab circula só dentro; Esc fecha; o foco volta ao controle de origem |

## O que conferir no seu design system

- Todo componente interativo tem a variante de foco desenhada.
- O token de foco tem 3:1 contra os fundos onde aparece, nos dois modos.
- O anel fica por fora do componente, com folga.
