# Usuários

Esta seção explica como o administrador gerencia as contas da plataforma:
listar, buscar, filtrar, abrir os detalhes de uma pessoa, editar seus dados e
consultar a assinatura e os pagamentos dela.

## Para que serve esta tela

A tela **Usuários** (menu lateral **Usuários**, endereço `/dashboard/usuarios`)
mostra todas as contas cadastradas — pessoas físicas e organizações. A partir
dela você visualiza, filtra, edita e remove usuários. O subtítulo da tela
resume: *"Visualize, filtre, edite e remova usuários da plataforma."*

## A lista de usuários

Cada usuário aparece como um cartão (ou linha de tabela) com:

- A **foto** (ou as iniciais do nome, quando não há foto).
- O **nome** e o **e-mail**.
- Três etiquetas coloridas:
  - **Papel**: "Administrador" ou "Usuário".
  - **Tipo de conta**: PF, PJ, PF + PJ (dual) ou — (sem perfil).
  - **Assinatura**: "Ativa", "Pendente", "Expirada", "Cancelada" ou "Sem plano".

Você pode alternar entre a visão em **cartões** e em **tabela**, e escolher
quantos itens carregar por vez (controle de tamanho de página no canto da lista).
No fim da lista há o botão para **carregar mais** resultados.

Clicar em qualquer usuário (cartão ou linha) abre a tela de **detalhes** dele.

## Buscar e filtrar

No topo da lista há a barra de filtros:

1. **Buscar** — digite parte do **nome ou e-mail** no campo de busca.
2. Abra os filtros avançados para refinar por:
   - **Papel** — "Todos", "Usuário" ou "Administrador".
   - **Tipo** — "Todos", "PF", "PJ (inclui dual)", "Dual (PF+PJ)" ou "Sem perfil".
   - **Assinatura** — "Todos", "Ativa", "Pendente", "Expirada", "Cancelada" ou
     "Sem plano".
3. Clique em **Filtrar** para aplicar.
4. Use **Limpar** para zerar todos os filtros e voltar à lista completa.

O contador ao lado dos filtros mostra quantos filtros avançados estão ativos.

## Ver os detalhes de um usuário

Ao clicar em um usuário, abre a tela de detalhes (endereço
`/dashboard/usuarios/[número]`), organizada em blocos:

- **Dados do usuário** — id, e-mail, tipo de conta, papel, nome, sobrenome,
  empresa atual, grau de instrução, informações de diversidade, data de cadastro,
  última atualização, situação do aceite da política de privacidade e a
  biografia.
- **Empresa** (apenas para contas PJ) — dados da organização (nome, razão
  social, CNPJ, setor, porte, site, contato) e a lista de **membros** vinculados,
  com status de cada um.
- **Assinatura atual** — plano, situação, datas de início e fim e o pagamento
  associado (ou a indicação de que foi atribuída manualmente pelo administrador).
- **Histórico de pagamentos** — tabela com data, plano, forma de pagamento,
  valor, status e provedor. Há um atalho **"Ver todos"** que leva à tela de
  Pagamentos já filtrada por aquele usuário.
- **Histórico de pagamentos legado (sistema antigo)** — registros vindos do
  sistema anterior, quando existirem.

No topo dos detalhes há o botão **Voltar** (retorna à lista) e o botão
**Editar usuário**.

## Editar um usuário

1. Na tela de detalhes, clique em **Editar usuário** (ou acesse
   `/dashboard/usuarios/[número]/editar`).
2. O formulário tem quatro blocos:
   - **Metadados** (somente leitura) — id, tipo de conta, situação da assinatura
     (com atalho para a tela de assinaturas), datas de cadastro e atualização.
   - **Identificação** — Nome, Sobrenome, E-mail e **Papel** (escolha entre
     "Usuário" e "Administrador").
   - **Contato profissional** — Empresa atual, Grau de instrução e Biografia.
   - **Diversidade** — Identidade de gênero, Orientação sexual, Cor/Raça,
     População tradicional e Informação de deficiência.
3. Clique em **Salvar** para gravar, ou **Cancelar** para descartar.

> O e-mail é validado: se não for um endereço válido, aparece um aviso e o salvamento é bloqueado.
> O tipo de conta (PF/PJ) **não** é editável aqui — é definido no cadastro.
> Os links de redes sociais (LinkedIn, Lattes etc.) também não são editados nesta
> tela administrativa; eles vivem no "Meu perfil" do próprio usuário.

## Assinatura e pagamentos do usuário

A assinatura e o histórico de pagamentos **são apenas para consulta** nesta área
de detalhes — servem para você entender a situação financeira da conta. Para
**atribuir, alterar ou cancelar** um plano de fato, use as telas dedicadas:
**Planos** (`/dashboard/planos`) e **Pagamentos** (`/dashboard/pagamentos`),
acessíveis pelo menu lateral.

## Remover um usuário

Ao acionar a remoção de um usuário, abre uma **janela de confirmação** antes de
apagar. A exclusão é definitiva e o sistema cuida de desfazer os vínculos
relacionados. O sistema impede que você remova a **própria conta**.
