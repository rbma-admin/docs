# Planos

## Para que serve esta seção

A seção **Planos** é onde você gerencia os planos de assinatura da plataforma. Um plano define o preço, o tipo de conta (pessoa física ou jurídica) e — o mais importante — **quais recursos** o assinante daquele plano passa a ter acesso.

Para abrir, clique em **Planos** no menu lateral.

A tela mostra um cartão para cada plano, lado a lado. Acima dos cartões há dois controles:

- **Ver assinantes ativos** — leva à lista de quem tem plano ativo (ver o manual de *Assinantes*).
- **Mostrar inativos** — uma caixinha para também exibir planos que foram arquivados.
- **Novo plano** — botão azul para criar um plano.

---

## O plano gratuito (base) e os planos pagos

Existem dois tipos de cartão na tela:

- **Conta gratuita (baseline)** — destacado em amarelo. É a configuração padrão de **todo usuário autenticado** que não tem assinatura paga. As permissões dele (ver o próprio perfil, gerenciar a própria assinatura, participar de organizações) são "implícitas": valem para todo mundo automaticamente. Por isso elas **não** aparecem repetidas nos planos pagos — para não poluir a tela.
- **Planos pagos** — cartões brancos, um para cada plano (Pessoa Física, Pessoa Jurídica, etc.). Mostram o preço, o status (Ativo/Inativo) e a lista de recursos que aquele plano libera além do baseline gratuito.

Cada cartão tem o link **Detalhes do plano**, que abre a página completa do plano.

> **Termos:** *Pessoa Física (PF)* é uma conta de indivíduo; *Pessoa Jurídica (PJ)* é uma conta de empresa/organização.

---

## Criar um plano

1. Clique em **Novo plano**.
2. Preencha o formulário:
   - **Código** — identificador interno, só com letras minúsculas, números e hífen (entre 3 e 40 caracteres). Ex.: `apoiador-pf`. **Não pode ser alterado depois.**
   - **Nome** — nome que aparece para o assinante (entre 2 e 120 caracteres).
   - **Preço (R$)** — valor da assinatura (use 0 ou mais).
   - **Tipo** — escolha **Pessoa física** ou **Pessoa jurídica**.
   - **Descrição** — texto opcional (até 500 caracteres).
3. Clique em **Salvar**.

O plano é criado já como **Ativo**. Em seguida, abra os **Detalhes do plano** para marcar quais recursos ele libera (ver abaixo).

---

## Editar um plano

1. No cartão do plano, clique em **Detalhes do plano**.
2. Na seção "Dados do plano", clique em **Editar**.
3. Você pode mudar **Nome**, **Preço** e **Descrição**. O **Código** e o **Tipo** ficam bloqueados (não podem mudar após a criação).
4. No modo de edição também aparece a caixa **Ativo** — desmarcá-la equivale a arquivar o plano.
5. Clique em **Salvar**.

---

## Definir os recursos (permissões) de um plano

Na página de **Detalhes do plano**, abaixo dos dados, fica a seção **Permissões liberadas pelo plano**.

1. A área mostra os recursos agrupados por tema, cada um com uma caixinha.
2. **Marque** a caixinha para liberar aquele recurso aos assinantes do plano; **desmarque** para retirar.
3. Cada mudança é salva na hora.

Observação: os recursos exclusivos de administrador (RBAC) **não** aparecem aqui — eles ficam na seção **Permissões** do menu. Aqui você só controla o que os assinantes pagantes recebem.

---

## Arquivar e reativar um plano

**Arquivar** tira o plano da lista padrão e impede novas atribuições, mas **não afeta** as assinaturas que já estão em vigor.

1. Abra **Detalhes do plano**.
2. Clique em **Arquivar**.
3. Confirme na janela "Arquivar plano" (o aviso explica: *"Ele sai da listagem default e não aceita novas atribuições. Assinaturas em vigor não são afetadas."*).
4. Clique em **Confirmar**.

Para trazer de volta um plano arquivado:

1. Marque **Mostrar inativos** na tela principal de Planos (ou abra o plano direto).
2. Abra os **Detalhes do plano** e clique em **Reativar**.

---

## Por que o plano base (gratuito) não pode ser arquivado

O plano gratuito é **estrutural**: ele define o que toda conta recebe ao se cadastrar, mesmo sem pagar nada. Quando uma assinatura paga expira, o usuário volta para esse plano base. Como ele é a fundação de todas as contas, a plataforma **não permite arquivá-lo nem excluí-lo**.

Ao abrir os detalhes do plano base, você verá um aviso amarelo explicando isso. Os botões de **Arquivar/Reativar** não aparecem para ele, e o preço é sempre exibido como **Gratuito**. Você ainda pode editar o **Nome** e a **Descrição**, mas o preço e o tipo permanecem fixos.
