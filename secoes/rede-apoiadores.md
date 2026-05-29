# Rede de Apoiadores

## Para que serve esta tela

A **Rede de Apoiadores** é o **diretório de profissionais** da RBMA: uma lista
pesquisável de pessoas (e empresas) que apoiam a rede e optaram por se mostrar.
Serve para que os apoiadores se encontrem, conheçam quem trabalha com
monitoramento e avaliação, e descubram empresas e instituições parceiras.

Ela existe em dois lugares:

- **Dentro do painel** — em **CONTEÚDO → Rede de Apoiadores**
  (endereço `/dashboard/rede`), com **filtros completos**. É a tela que este
  manual descreve em detalhe.
- **Na página pública** — em `/rede` no site, aberta a apoiadores com acesso. É
  a "vitrine" da rede. Os perfis individuais públicos ficam em `/rede/:id`.

> Acesso por plano: a Rede de Apoiadores depende de uma **assinatura ativa** que
> inclua esse recurso. Quem não tem o acesso vê uma tela informando que *"Seu
> plano não inclui a Rede de Apoiadores"*.

---

## Quem aparece na Rede (o opt-in "Aparecer na Rede")

Ninguém entra no diretório sem permitir. Cada pessoa física controla isso no
próprio perfil:

1. Em **Perfil → Editar perfil**, há a seção **"Rede de Apoiadores"**.
2. Lá existe a opção **"Aparecer na Rede de Apoiadores"** (uma caixa de marcar).
3. Quando marcada, o perfil passa a ser **visível** para outros apoiadores em
   `/rede`. A pessoa pode **desmarcar a qualquer momento** e sair do diretório.

Resumindo: **só aparece na Rede quem ligou essa opção**. Por isso, a tela diz
que lista "os apoiadores PF da rede que optaram por aparecer no diretório".

> No caso das **empresas (PJ)**, não há essa caixinha: uma organização aparece na
> Rede automaticamente quando tem o plano que dá acesso ao recurso.

---

## A lista de apoiadores

A tela **"Rede de Apoiadores"** mostra os apoiadores em **cards** (cartões) ou
em **tabela** — alterne pelo controle no canto direito da barra de filtros. Cada
apoiador exibe **foto** (ou iniciais), **nome**, **e-mail**, **empresa atual**,
**instituição** e etiquetas indicando se tem **Lattes** e/ou **LinkedIn**.

- Logo acima da lista há um resumo no formato **"X de Y"** (quantos estão
  carregados de quantos no total).
- Use o botão de **carregar mais** ao final para trazer mais resultados.
- Clique num apoiador para abrir o **perfil de detalhe** dele dentro do painel
  (endereço `/dashboard/rede/:id`).

---

## Os filtros

No topo há o campo de **busca** (por **nome ou e-mail**) e um botão
**"Filtros"** que abre os filtros avançados. Os filtros do painel são bem ricos.

### Filtros de texto (digite parte do termo)

- **Empresa atual** (ex.: "RBMA")
- **Grau de instrução** / instituição educacional (ex.: "USP")
- **Identidade de gênero**
- **Orientação sexual**
- **Cor / raça**
- **População tradicional**
- **PCD / informação de deficiência**

> Esses filtros funcionam por correspondência parcial: basta digitar um trecho
> do que procura.

### Filtros de "tem ou não tem" (três opções)

Para cada um, escolha **Qualquer**, **Com** ou **Sem**:

- **Lattes** (currículo Lattes preenchido)
- **LinkedIn**
- **Foto de perfil**
- **Biografia**

### Filtros por lista (escolha numa caixa de seleção)

- **País** e **Estado** (o estado aparece conforme o país escolhido)
- **Área de atuação**: Academia, Terceiro setor, Governo, Consultoria ou Outra
- **Nível de experiência em M&A** (monitoramento e avaliação): Iniciante,
  Intermediário ou Avançado
- **Tipo de apoiador**: Todos, Pessoas (PF) ou Empresas (PJ)

### Aplicar e limpar

- Ajuste os filtros e aplique para atualizar a lista.
- O botão **"Limpar todos os filtros"** reseta tudo. O número ao lado de
  **"Filtros"** indica quantos filtros avançados estão ativos no momento.

---

## A página pública `/rede`

Além da versão do painel, existe a página pública **`/rede`**, que é a vitrine
da Rede de Apoiadores no site. Ela apresenta os mesmos apoiadores que optaram por
aparecer, e cada perfil pode ser aberto em **`/rede/:id`**.

Os links **"Ver na Rede"** (na lista de participantes de uma empresa) e
**"Ver meu perfil na Rede de Apoiadores"** (no perfil da pessoa ou da empresa)
levam justamente para essa página pública, abrindo o perfil correspondente.

---

## Resumo rápido

- A Rede de Apoiadores é um **diretório de profissionais e empresas** da RBMA.
- Uma pessoa só aparece se **marcar "Aparecer na Rede de Apoiadores"** em
  *Editar perfil*; empresas aparecem pelo **plano** que dá acesso.
- No painel (**CONTEÚDO → Rede de Apoiadores**) há **busca** e filtros completos:
  empresa, instituição, recortes de diversidade, **com/sem Lattes, LinkedIn,
  foto e biografia**, país, estado, área de atuação, experiência e tipo (PF/PJ).
- A versão pública fica em **`/rede`**; cada perfil em **`/rede/:id`**.
- O acesso ao recurso depende de uma **assinatura ativa** que o inclua.
