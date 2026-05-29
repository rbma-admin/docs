# Templates de e-mail

## Para que serve esta tela

A plataforma envia e-mails automáticos em vários momentos: quando alguém pede
para redefinir a senha, quando um convite é aceito, quando um pagamento é
confirmado, quando uma assinatura está prestes a vencer, e assim por diante.
Cada um desses e-mails automáticos é chamado de **template** (modelo).

Nesta tela você pode **ler, editar e personalizar** o texto desses e-mails sem
precisar de ajuda técnica: muda o assunto, o conteúdo e até desliga (pausa) os
e-mails que não são obrigatórios. Você também pode **enviar um teste para si
mesmo** antes de publicar qualquer mudança.

Onde fica: no menu lateral, em **GESTÃO → Templates de e-mail**
(endereço `/dashboard/comunicacoes/templates`). É uma seção só para
administradores.

---

## A lista de templates

Ao abrir a seção, você vê a tela **"Templates de e-mail"**. Os modelos vêm
organizados em quatro grupos (categorias), nesta ordem:

1. **Segurança** — e-mails ligados ao login e à conta (redefinição de senha,
   senha alterada, confirmação de e-mail).
2. **Vínculos PJ** — e-mails sobre organizações e membros (convite para entrar
   numa empresa, aviso de novo membro, aviso de saída de membro, empresa
   removida).
3. **Pagamento** — e-mails de cobrança (pagamento confirmado, pagamento
   recusado, boleto gerado).
4. **Ciclo de assinatura** — avisos sobre a assinatura (assinatura prestes a
   vencer, assinatura vencida, assinatura cancelada).

> A lista é montada automaticamente a partir do sistema. Se no futuro um novo
> tipo de e-mail for adicionado, ele aparece aqui sozinho, sem precisar de
> ajuste.

### O que cada linha mostra

Em cada modelo da lista você verá:

- O **assunto atual** do e-mail.
- Uma etiqueta **"Padrão"** (ainda usa o texto original do sistema) ou
  **"Customizado"** (você já editou esse modelo).
- Quando foi a **última atualização** (ex.: "há 3 dias").
- Um interruptor **Ativo / Pausado** para ligar ou desligar o envio.
- Um link **"Editar"** para abrir o editor.

Se por acaso aparecer uma etiqueta amarela **"⚠ Erro de render — usando
default"**, significa que o sistema teve um problema ao montar a sua versão
personalizada e, por segurança, voltou a usar o texto original. Abra o modelo,
revise o conteúdo e salve novamente.

### Ligar e desligar um e-mail

1. Localize o modelo na lista.
2. Clique no interruptor **Ativo / Pausado** ao lado dele.
3. A mudança vale na hora. Quando "Pausado", aquele e-mail deixa de ser enviado.

#### Regra importante: e-mails de segurança não podem ser desligados

Os modelos do grupo **Segurança** (redefinição de senha, senha alterada,
confirmação de e-mail) ficam **sempre ativos**. O interruptor deles aparece
travado e, ao passar o mouse, mostra o aviso *"E-mail de segurança — sempre
ativo"*. Isso é proposital: desligar esses e-mails impediria as pessoas de
recuperar a conta ou de se cadastrar com segurança. Você ainda pode **editar o
texto** desses modelos — só não pode desativá-los.

---

## Editando um template

1. Na lista, clique em **"Editar"** no modelo desejado (ou clique no nome).
2. A tela do editor abre dividida em duas colunas: à esquerda o **Editor**, à
   direita o **Preview** (pré-visualização). Em celular, use as abas **Editor**
   e **Preview** no topo para alternar.

No lado do **Editor** há três campos:

- **Assunto (subject)** — o título que a pessoa vê na caixa de entrada.
- **HTML** — o corpo do e-mail com formatação (cores, links, negrito). É o que
  a maioria das pessoas enxerga.
- **Texto plano** — uma versão simples, sem formatação, usada por programas de
  e-mail que não exibem HTML.

Para alterar, basta clicar no campo e digitar. Não é obrigatório preencher os
três: você precisa preencher **pelo menos um** (assunto, HTML ou texto). Se
deixar tudo vazio, o sistema avisa *"Preencha ao menos um dos campos"*.

### Variáveis (os dados que entram automaticamente)

Cada e-mail tem alguns **dados dinâmicos** que são preenchidos na hora do envio
— por exemplo, o nome da empresa, o valor pago ou o link para redefinir a
senha. Esses dados aparecem como **variáveis**, em chips (botõezinhos) logo
abaixo dos campos, com nomes claros como *"Nome da empresa"*, *"Valor pago"* ou
*"Link para redefinir senha"*.

Para usar uma variável:

1. Clique dentro do campo onde quer inserir (Assunto, HTML ou Texto) e deixe o
   cursor na posição desejada.
2. Clique no chip da variável. Ela é inserida exatamente onde estava o cursor.

Cada modelo só aceita as variáveis listadas para ele. Se você digitar à mão uma
variável que não existe naquele modelo, ao salvar o sistema avisa *"Variáveis
não permitidas"* e lista quais. Use sempre os chips para evitar erro.

> No bloco **"Ajustar dados do preview"** você pode trocar os valores de exemplo
> usados na pré-visualização (ex.: testar com outro nome de empresa). Isso afeta
> só o preview, não o e-mail real.

### Pré-visualização (Preview)

A coluna da direita mostra, em tempo real, **como o e-mail vai ficar** com o
texto que você está escrevendo. Ela atualiza sozinha alguns instantes após você
parar de digitar. Se algum dado obrigatório estiver faltando, o preview avisa.

### Ligar / pausar dentro do editor

No rodapé da coluna do editor há uma caixinha **Ativo / Pausado**, igual à da
lista. Em modelos de segurança ela aparece travada (sempre ativo).

### Salvar ou cancelar

- Clique em **Salvar** para publicar as mudanças. Uma mensagem confirma
  *"Template salvo"*.
- Clique em **Cancelar** para voltar sem salvar.
- Se você tentar sair com alterações não salvas, aparece um aviso perguntando
  se quer **Descartar** ou **Continuar editando**.

---

## Enviar um teste para você mesmo

Antes de confiar numa mudança, teste:

1. Na coluna da direita do editor, clique em **"Enviar teste para mim"**.
2. O sistema envia o e-mail para o **seu próprio endereço** (o e-mail da sua
   conta de administrador). Uma mensagem confirma o envio.
3. Abra sua caixa de entrada e veja como o e-mail chegou de verdade.

Observações:

- Se você enviar muitos testes seguidos, o sistema pede para **aguardar alguns
  segundos** antes de tentar de novo (proteção contra excesso de envios).
- Se o seu e-mail de administrador ainda **não estiver confirmado**, o teste é
  bloqueado e aparece um atalho **"Reenviar e-mail de verificação"**. Confirme
  seu e-mail e tente novamente.

---

## Restaurar o texto original (Restaurar padrão)

Se você se arrepender das mudanças e quiser **voltar ao texto original** do
sistema:

1. No editor, clique em **"Restaurar padrão"**.
2. Como a ação é definitiva, o sistema pede que você **digite a palavra
   `RESTAURAR`** para confirmar.
3. Clique em **Restaurar**. Sua personalização daquele modelo é descartada e o
   texto volta ao original.

> Atenção: isso apaga de vez a sua versão personalizada daquele modelo. Não dá
> para desfazer.

---

## Layout global (cabeçalho e rodapé de todos os e-mails)

Todos os e-mails da plataforma compartilham um **cabeçalho (header)** no topo e
um **rodapé (footer)** no final — normalmente o logo, cores e informações de
contato da RBMA. Em vez de repetir isso em cada modelo, você edita esse moldura
uma única vez, no **Layout global**.

1. Na tela da lista de templates, clique no link **"Layout global"** (canto
   superior direito). Ou acesse `/dashboard/comunicacoes/layout`.
2. Você verá dois campos: **Header HTML** (cabeçalho) e **Footer HTML**
   (rodapé). A coluna da direita mostra o **preview** de como fica.
3. Edite o conteúdo e clique em **Salvar**.

Detalhes:

- O cabeçalho e o rodapé são **HTML literal**, **sem variáveis dinâmicas** —
  aqui não há chips de variáveis.
- Há também um botão **"Restaurar padrão"** que devolve o layout original
  (mesma confirmação por palavra digitada).
- A etiqueta **"Padrão"** ou **"Customizado"** indica se o layout já foi
  alterado.

---

## Resumo rápido

- **GESTÃO → Templates de e-mail**: lista dos modelos por categoria.
- Edite **Assunto / HTML / Texto plano**; use os **chips de variáveis** para
  inserir dados automáticos.
- **Preview** mostra o resultado; **Enviar teste para mim** manda uma cópia real
  para você.
- E-mails de **Segurança** podem ser editados, mas **nunca desativados**.
- **Restaurar padrão** desfaz a personalização (ação definitiva).
- **Layout global** controla o cabeçalho e rodapé de todos os e-mails de uma só
  vez.
