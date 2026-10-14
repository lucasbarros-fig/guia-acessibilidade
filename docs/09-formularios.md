# 9. Formulários

`WCAG 1.3.5, 3.3.1, 3.3.2, 3.3.7, 3.3.8 e 4.1.2 · NBR 5.9`

Todo campo tem um rótulo visível acima dele. O texto de exemplo dentro do campo some ao digitar e nunca é rótulo.

## Regras

- **Rótulo visível:** sempre, inclusive em busca. Se o design system tem um campo sem rótulo, ele serve só com um rótulo visível por perto ligado ao campo. `NBR 5.9.1 a 5.9.4`
- **Formato esperado:** escrito no texto de ajuda, visível antes de digitar (“DD/MM/AAAA”, “pelo menos 8 caracteres”). `NBR 5.9.5`
- **Obrigatório:** marcado por texto ou símbolo explicado, nunca só pela cor. `NBR 5.9.7`
- **Erro:** ícone, texto e cor, logo abaixo do campo, dizendo como resolver. “Informe um e-mail válido, como nome@empresa.com.br” em vez de só “E-mail inválido”. `NBR 5.9.9 e 5.9.10`
- **Campo desabilitado:** pode ficar apagado; o contraste de desabilitado é isento. Se a pessoa precisa ler ou copiar o dado (CPF, CNPJ), use **somente leitura** em vez de desabilitado.
- **Preenchimento automático:** marque o propósito do campo. E-mail de login = `username`; senha atual = `current-password`; senha nova = `new-password`; código = `one-time-code`. `WCAG 1.3.5`
- **Colar liberado** em senha e código. Login sem teste cognitivo: nada de digitar caracteres de uma imagem sem alternativa. `WCAG 3.3.8 · NBR 5.9.18`
- **Código de verificação em caixas:** um grupo com nome (“Código de verificação”); colar o código inteiro preenche todas as caixas; a contagem (“Expira em 4:59”) é anunciada em marcos, nunca a cada segundo.
- **Nada digitado duas vezes:** dado que a pessoa já informou no fluxo aparece preenchido. A confirmação de senha é a exceção. `WCAG 3.3.7 · NBR 5.9.15`
- **Formulário que tem consequência** (financeiro, jurídico, envio de dados): permitir revisar, corrigir ou cancelar antes de confirmar. `NBR 5.9.12`

## O que conferir no seu design system

- O campo padrão traz rótulo, texto de ajuda e erro com ícone.
- Existe o estado somente leitura, diferente do desabilitado.
- O erro não depende só da cor da borda.
