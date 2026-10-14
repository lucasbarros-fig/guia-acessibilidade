# 12. Movimento e tempo

`WCAG 2.2.1, 2.2.2, 2.3.1 e 2.3.3 · NBR 5.15 e 5.16`

Tudo que anima tem uma versão parada para quem ativa “reduzir movimento” no sistema, e nada muda de tela ou some antes de a pessoa ler.

## Regras

- **Reduzir movimento:** desenhe a versão parada de cada animação. Exemplos: skeleton sem brilho, abertura sem deslocamento do logotipo, carregamento sem giro.
- **Movimento automático:** o que se move por mais de 5 s tem botão de pausa. `WCAG 2.2.2 · NBR 5.15.1`
- **Nada pisca** mais de 3 vezes por segundo. `WCAG 2.3.1 · NBR 5.15.4`
- **Mensagens temporárias:** sem ação, cerca de 6 s na tela, mais para texto longo. Com ação, ficam até serem dispensadas.
- **Nada volta sozinho:** uma tela de sucesso não leva a outra tela por tempo. Use um botão (“Ir para o login”).
- **Prazos:** sessão ou código que expira avisa antes e oferece como estender (“Reenviar código”). `WCAG 2.2.1 · NBR 5.16.2`

## O que conferir no seu design system

- Componentes animados (skeleton, carregamento, carrossel, toast) têm a variante sem movimento.
- O tempo padrão dos toasts.
