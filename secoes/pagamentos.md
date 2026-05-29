# Pagamentos

## Para que serve esta seção

A seção **Pagamentos** é o histórico de **todas as transações financeiras** do sistema — cada cobrança de assinatura feita por qualquer usuário. É uma tela de **acompanhamento (somente leitura)**: você consulta e filtra os pagamentos, mas não edita nem estorna nada por aqui.

Para abrir, clique em **Pagamentos** no menu lateral.

---

## A lista de transações

A tela mostra a seção **Transações** com uma tabela. No computador, cada linha traz as colunas:

- **Data** — quando o pagamento foi criado.
- **User ID** — o número do usuário que fez o pagamento (clicável: leva à ficha do usuário).
- **Plano** — o plano associado (Pessoa Física ou Pessoa Jurídica).
- **Método** — a forma de pagamento (ver explicação abaixo).
- **Valor** — em reais. Pagamentos reembolsados aparecem riscados.
- **Status** — uma etiqueta colorida (ver significados abaixo).
- **Provedor** — quem processou o pagamento (Mercado Pago, PayPal ou Admin).

No celular, cada transação aparece como um cartão com as mesmas informações.

No alto da lista, o sistema indica a **página atual** e o **total** de transações. Use os botões **Anterior** e **Próxima** no rodapé para navegar entre as páginas.

---

## Filtrar pagamentos

Os filtros ficam logo abaixo do título. Eles são aplicados imediatamente ao escolher uma opção.

1. **Status** — Todos, Pendente, Sucesso, Falhou, Cancelado ou Reembolsado.
2. **Provedor** — Todos, PayPal, Mercado Pago ou Admin (manual).
3. **Plano** — Todos, Pessoa Física ou Pessoa Jurídica.
4. **ID do usuário** — digite o número de um usuário para ver só os pagamentos dele (opcional).

Para limpar tudo de uma vez, use **Limpar filtros**.

---

## O que significa cada status

- **Pendente** (amarelo) — o pagamento foi iniciado mas ainda não foi confirmado. É o caso típico de Pix ou boleto aguardando compensação.
- **Sucesso** (verde) — o pagamento foi confirmado e a assinatura está paga.
- **Falhou** (vermelho) — a tentativa de pagamento não deu certo (ex.: cartão recusado).
- **Cancelado** (cinza) — o pagamento foi cancelado antes de ser concluído.
- **Reembolsado** (cinza) — o valor foi devolvido ao usuário. Nesses casos o valor aparece riscado na tabela.

---

## O que significa cada método de pagamento

A coluna **Método** indica como o usuário pagou:

- **Cartão** — pagamento com cartão de crédito.
- **Pix** — pagamento instantâneo brasileiro, feito por QR Code ou chave; cai na hora.
- **Boleto** — boleto bancário; o usuário paga em banco/app e a confirmação leva de horas a alguns dias úteis (por isso fica "Pendente" até compensar).
- **PayPal** — pago pela conta PayPal.
- **Mercado Pago** — pago pela plataforma Mercado Pago.
- **Admin** — não foi uma cobrança real: o plano foi atribuído manualmente por um administrador (sem pagamento).

> **Termos:** *Pix* é o sistema de transferência instantânea do Banco Central; *boleto* é o documento de cobrança bancária tradicional.

---

## Mercado Pago e PayPal

A plataforma trabalha com dois processadores de pagamento ("provedores"):

- **Mercado Pago** — é o provedor **principal e ativo**. É por ele que passam os pagamentos com Cartão, Pix e Boleto.
- **PayPal** — está atualmente **desativado**. Por decisão de configuração, a opção de pagar com PayPal não é mais oferecida aos usuários no momento da contratação — apenas o Mercado Pago aparece.

Mesmo com o PayPal desativado, você ainda pode encontrar transações antigas marcadas como "PayPal" no histórico (são de quando ele estava ativo). O filtro de **Provedor** continua oferecendo PayPal justamente para você localizar essas transações passadas.
