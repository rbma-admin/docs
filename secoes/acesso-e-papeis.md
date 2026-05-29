# Acesso e papéis

Esta seção explica como entrar e sair do painel administrativo, quais são os
dois tipos de usuário (administrador e usuário comum), os dois tipos de conta
(Pessoa Física e Pessoa Jurídica) e o que cada um enxerga ao acessar o sistema.

## Para que serve esta tela

A tela de **Login** é a porta de entrada do painel. Tudo que está sob o
endereço `/dashboard` exige que você esteja autenticado(a). Quem não está logado
é levado automaticamente para a tela de login.

## Como entrar (login)

1. Acesse a página de login (botão **Login** no topo do site, ou o endereço
   `/login`).
2. Preencha o campo **E-mail** (placeholder "Digite seu e-mail").
3. Preencha o campo **Senha** (placeholder "Digite sua senha").
4. Clique no botão **Login**.
5. Se as credenciais estiverem corretas, você é levado(a) ao painel. Se estiverem
   erradas, aparece a mensagem **"E-mail ou senha incorretos."**.

Na mesma tela existem dois atalhos:

- **Esqueci a senha** — leva à tela de recuperação (veja a observação abaixo).
- **Cadastre-se!** — leva à tela de criação de conta.

## Como sair (logout)

O botão de sair fica no menu/cabeçalho do painel, junto ao seu nome. Ao sair,
sua sessão é encerrada e você volta para a tela de login. Por segurança, sempre
saia ao usar um computador compartilhado.

## Duração da sessão (expiração em 24 horas)

- A sessão tem validade de **24 horas**.
- Quando a sessão expira (ou se ela é encerrada por outro motivo), o sistema
  desconecta você automaticamente e exibe a mensagem **"Sua sessão expirou. Faça
  login novamente."**, redirecionando para a tela de login.
- **Não existe "renovação automática" visível ao usuário**: ao expirar, basta
  fazer login de novo.

## Os dois papéis: Administrador x Usuário

Cada conta tem um **papel** (também chamado de "role"), que define o que a pessoa
pode ver e fazer:

- **Administrador** — enxerga o painel completo: gestão de Usuários,
  Organizações, Pagamentos, Planos, Permissões, Notícias, Cursos, Seminários,
  Eventos, Biblioteca, Templates de e-mail, Mensagens de contato e a Rede de
  Apoiadores. O administrador tem acesso a **tudo** automaticamente.
- **Usuário** (comum) — enxerga apenas o necessário para a própria conta:
  o **Perfil**, suas **Minhas assinaturas** e, dependendo do plano contratado,
  a Biblioteca e a Rede de Apoiadores. Não vê nenhuma tela de gestão.

> Importante: o papel é o que dá (ou não) acesso às telas administrativas. Mesmo
> que alguém digite manualmente o endereço de uma tela de gestão, sem o papel
> correto verá uma tela de bloqueio explicando que não tem permissão.

## Os dois tipos de conta: Pessoa Física (PF) e Pessoa Jurídica (PJ)

Além do papel, cada conta tem um **tipo**, escolhido no cadastro:

- **Pessoa Física (PF)** — uma pessoa individual. No cadastro pede Nome,
  Sobrenome, e-mail, senha e dados opcionais (empresa atual, grau de instrução,
  biografia e perguntas de diversidade).
- **Pessoa Jurídica (PJ)** — uma organização. No cadastro pede Nome da
  organização, Pessoa para contato, Cargo da pessoa para contato, **CNPJ**,
  e-mail e senha.

O tipo de conta muda o que a pessoa vê no menu lateral:

- A conta **PF** vê o painel pessoal: Dashboard, Perfil e suas assinaturas.
- A conta **PJ** vê o painel da organização: Dashboard, Participantes
  (membros), Perfil da organização e suas assinaturas.

Existe ainda uma situação especial chamada **Dual (PF+PJ)**: é uma pessoa física
que também faz parte de uma organização. Para fins de uso do sistema, ela é
tratada como **PF** (vê o menu de pessoa física), com a adição da tela "Minhas
organizações". Esse rótulo "Dual" aparece, por exemplo, no filtro de tipo na
tela de Usuários.

> O **tipo de conta** (PF/PJ) é uma questão de experiência de uso — define qual
> menu a pessoa vê. O **papel** (admin/usuário) é o que controla permissões de
> verdade. Uma conta pode ser, por exemplo, PF e administradora ao mesmo tempo.

## Criar conta (cadastro)

A tela de cadastro tem duas etapas:

1. **1. Informações de Cadastro** — escolha entre **Pessoa Física** e **Pessoa
   Jurídica** no seletor de tipo, preencha os dados e a senha (mínimo de 8
   caracteres), e marque o aceite da **Política de Privacidade**.
2. **2. Diversidade** — perguntas opcionais (identidade de gênero, orientação
   sexual, cor/raça, população tradicional e deficiência), exibidas apenas para
   Pessoa Física.

Ao concluir, aparece **"Cadastro realizado. Verifique seu e-mail."** — a conta
precisa ser confirmada por e-mail antes do primeiro login.

## Recuperação de senha (situação atual)

A tela **Esqueci a senha** existe e mostra uma mensagem de confirmação ao
informar o e-mail. **Atenção:** o fluxo de redefinição de senha por e-mail ainda
não está totalmente disponível no sistema. Enquanto isso, a forma garantida de
trocar a senha de um usuário é o administrador atuar diretamente (suporte
manual). Se um usuário relatar que não recebeu o e-mail de redefinição, oriente-o
a procurar o administrador.
