# Organizações (contas Pessoa Jurídica) e membros

## Para que serve esta seção

Na RBMA existem dois tipos de conta:

- **Pessoa Física (PF)** — uma pessoa, com perfil individual.
- **Pessoa Jurídica (PJ)** — uma **organização/empresa**, com nome fantasia,
  razão social, CNPJ, logo, e que pode ter **vários membros** (pessoas físicas)
  vinculados a ela.

Esta seção do manual cobre tudo o que envolve as contas PJ: como o
**administrador** acompanha as organizações cadastradas, como o **responsável
pela empresa** edita o perfil e gerencia os membros, e como uma **pessoa física**
enxerga as organizações de que faz parte.

> O **CNPJ** e o **e-mail** de uma conta PJ são imutáveis: eles identificam a
> conta e não podem ser trocados depois de criados.

---

## Parte 1 — Visão do administrador: "Organizações"

Onde fica: no menu lateral, em **GESTÃO → Organizações**
(endereço `/dashboard/organizacoes`). É uma seção só para administradores.

### A lista

A tela **"Organizações"** lista todas as contas PJ cadastradas na plataforma.
Você pode ver em dois formatos — **cards** (cartões) ou **tabela** —, alternando
pelo controle no canto direito da barra de filtros. Cada organização mostra:

- **Logo** (ou um ícone, quando não há logo).
- **Nome** (nome fantasia) e, abaixo, a **razão social**.
- **CNPJ**.
- **Setor** e **Porte** (Micro, Pequena, Média ou Grande), quando preenchidos.

### Buscar

Use o campo de busca no topo (**"Buscar por nome ou CNPJ…"**) e clique em buscar.
Para carregar mais resultados, use o botão de **carregar mais** ao final da
lista.

### Ver detalhes e excluir

- Clique numa organização para abrir a **página de detalhes** dela, onde você
  pode revisar e ajustar os dados.
- Para **remover** uma organização, use a opção de exclusão e confirme na janela
  **"Deletar organização"**. Essa ação é **irreversível** e remove também os
  vínculos dos membros daquela empresa.

---

## Parte 2 — Visão do responsável pela empresa (conta PJ)

Quando alguém entra com uma **conta PJ**, o menu lateral mostra o grupo
**EMPRESA**, com **Perfil** e **Participantes**.

### Perfil da empresa

Onde fica: **EMPRESA → Perfil** (endereço `/dashboard/empresa/perfil`).

Nesta tela única (**"Perfil da empresa"**) ficam reunidos:

- **Sua conta** (somente leitura): e-mail de contato, tipo de conta, plano e a
  data em que a conta foi criada.
- **Dados da empresa** (editáveis): logo, nome fantasia, razão social, CNPJ
  (bloqueado), site, setor, porte, pessoa para contato e cargo.
- **Detalhes**: descrição, interesses em avaliação e redes sociais.

Como editar:

1. Para trocar o **logo**, use o bloco **"Enviar logo"** no início dos dados da
   empresa. Aceita imagens **JPG, PNG ou WebP**, com até **5 MB**.
2. Preencha ou ajuste os campos desejados. O **CNPJ** aparece desabilitado (não
   é editável).
3. Marque os **interesses em avaliação** e adicione **redes sociais** se quiser.
4. Clique em **"Salvar alterações"**. Uma mensagem confirma a atualização.

> Quanto mais completo o perfil (site, porte, descrição, logo, redes sociais),
> maior a visibilidade da organização na Rede de Apoiadores.

### Participantes (membros da organização)

Onde fica: **EMPRESA → Participantes** (endereço `/dashboard/empresa/membros`).

A tela **"Participantes"** lista as pessoas vinculadas à organização, cada uma
com:

- **Foto** (ou iniciais) e **nome**.
- **E-mail**.
- Uma etiqueta de **Status**.
- A etiqueta **"Principal"** quando aquele é o vínculo principal do membro.

Os status possíveis de um membro são:

- **Pendente** — foi convidado, mas ainda não aceitou. Mostra a data em que o
  convite **expira**.
- **Ativo** — aceitou o convite e faz parte da organização. Mostra a data em que
  **entrou**.
- **Revogado** — o vínculo foi cancelado/removido.
- **Expirado** — o convite passou da validade sem ser aceito.

Use as abas **Todos / Pendente / Ativo / Revogado** no topo para filtrar.

#### Convidar um novo membro

1. Clique em **"Convidar membro"** (canto superior direito).
2. Na janela **"Convidar membro"**, digite o **e-mail do convidado**.
3. Clique em **"Enviar convite"**. A pessoa recebe um e-mail com um link para
   aceitar. Enquanto não aceita, o membro fica como **Pendente**.

> Se o e-mail já tiver sido convidado, o sistema avisa. Cada convite tem uma
> validade; convites não aceitos viram **Expirado**.

#### Reenviar convite ou remover um membro

Para **reenviar** o convite (a um membro pendente) ou **revogar/remover** um
membro, clique no participante para abrir a **página de detalhes dele**
(endereço `/dashboard/empresa/membros/:id`). É lá que ficam essas ações.
Revogar cancela o convite (se ainda pendente) ou desliga o membro (se ativo).

#### "Ver na Rede"

Se um membro ativo optou por aparecer na **Rede de Apoiadores**, surge ao lado
dele um atalho **"Ver na Rede"**, que abre o perfil público da pessoa. (Veja a
seção *Rede de Apoiadores* deste manual.)

---

## Parte 3 — Visão da pessoa física: "Minhas organizações"

Uma pessoa física (PF) pode pertencer a uma ou mais organizações. Ela acompanha
isso em:

Onde fica: **CONTA → Minhas organizações**
(endereço `/dashboard/minhas-organizacoes`).

A tela **"Minhas organizações"** lista as empresas onde a pessoa é membro, cada
uma com **logo**, **nome**, **status** do vínculo e a etiqueta **"Principal"**
na organização padrão. Se a pessoa ainda não faz parte de nenhuma, a tela mostra
*"Você ainda não faz parte de nenhuma organização."*

- Clicar numa organização **ativa** abre a **página de detalhes do vínculo**
  (endereço `/dashboard/minhas-organizacoes/:id`), onde a pessoa pode **definir
  como principal** ou **sair** daquela organização.
- Definir uma organização como **principal** marca-a como a padrão da pessoa
  (só uma pode ser a principal por vez).

### Como uma pessoa entra numa organização

1. Ela recebe um **e-mail de convite** enviado pelo responsável da empresa.
2. Ao clicar no link, vê uma prévia do convite e pode **aceitar** (precisa estar
   logada na conta cujo e-mail recebeu o convite).
3. Depois de aceitar, o vínculo fica **Ativo** e a empresa passa a aparecer em
   **Minhas organizações**.

---

## Resumo rápido

- **Conta PJ** = organização (nome, CNPJ, logo, membros). CNPJ e e-mail são
  imutáveis.
- **Administrador**: **GESTÃO → Organizações** — lista, busca, detalhes e
  exclusão de todas as empresas.
- **Responsável da empresa**: **EMPRESA → Perfil** (dados e logo) e **EMPRESA →
  Participantes** (convidar, reenviar, revogar membros).
- Status de membro: **Pendente, Ativo, Revogado, Expirado**.
- **Pessoa física**: **CONTA → Minhas organizações** — vê seus vínculos, define
  a **Principal** ou **sai** de uma organização.
