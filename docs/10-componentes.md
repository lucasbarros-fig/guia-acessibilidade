# 10. Componentes e padrões

`WCAG 1.3.1, 2.4.4, 4.1.2 e 4.1.3 · NBR 5.7, 5.8 e 5.13`

Cada componente tem um comportamento esperado que o desenho precisa mostrar e o código precisa seguir. Quando o design system traz o componente, use o do design system: peça feita à mão perde o comportamento.

| Componente | Regra |
| --- | --- |
| Link ou botão | Leva a outra tela = link (“Ver todas as notícias”). Executa uma ação = botão. O nome diz o resultado, nunca “clique aqui”. `NBR 5.7.4 e 5.8.3` |
| Botão só com ícone | Nome que diz a ação: “Fechar notificação”, “Recolher menu”, “Notificações, 3 não lidas”. Nunca o nome do ícone. `NBR 5.13.10` |
| Diálogo | Título visível e Fechar visível. Com dados digitados, confirmar antes de descartar (“Continuar editando” ou “Descartar alterações”) |
| Toast | Anunciado como status, sem mover o foco. Fechar como botão de ícone. Fica cerca de 6 s (mais para texto longo); com ação, fica até ser dispensado. Largura limitada à tela. `NBR 5.13.8` |
| Menu suspenso | Itens com estado de foco; grupos com nome |
| Abas | “Aba 1 de 4”, a selecionada marcada; o painel vem logo depois |
| Carrossel | Sem avanço automático (ou Pausar como primeiro controle). Anterior e Próximo com nome. Indicador atual por forma e “2 de 4”. Texto real, nunca dentro da imagem |
| Aviso de cookies | Não bloqueia a página e não fecha sozinho. “Recusar” com o mesmo peso de “Aceitar” (ou “Entendi”, se forem só cookies essenciais). Link sublinhado |
| Menu lateral | Item atual marcado. Recolhido: cada ícone tem nome e tooltip no foco. Em telas pequenas, a gaveta se comporta como diálogo |
| Perguntas em sequência (cascata) | Cada pergunta é um grupo de opções cujo nome é o título. Ao escolher, anunciar “Próxima pergunta: …” sem mover o foco. Avisar antes de apagar respostas seguintes |
| Tabela de dados | Cabeçalhos marcados como cabeçalho; tabela com título. `NBR 5.6` |
| Lista | Itens marcados como lista, não como parágrafos soltos. `NBR 5.5` |

## Para quem desenvolve

O desenho não mostra tudo. Estes pontos vêm do componente e precisam estar no código:

- **Nome acessível** em todo controle, igual ou começando pelo texto visível. `NBR 5.13.7 e 5.13.10`
- **Estado anunciado:** selecionado, expandido, marcado, desabilitado. `NBR 5.13.13`
- **Elemento nativo** sempre que existir (`button`, `a`, `input`), antes de qualquer componente customizado. `NBR 5.13.11`
- **Títulos e regiões** marcados (cabeçalho, navegação, conteúdo principal), com um título de página único. `NBR 5.3, 5.4 e 5.13.1`
- **Idioma da página** declarado. `NBR 5.13.2`
