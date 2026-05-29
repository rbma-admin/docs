# Permissões

Esta seção explica a tela de **Permissões**: o que são as permissões
("capabilities"), como elas se dividem entre as que vêm do papel de
administrador, as que todo usuário já tem por padrão (plano base) e as que
dependem do plano contratado, e onde de fato se libera ou bloqueia uma permissão.

## Para que serve esta tela

A tela **Permissões** (menu lateral **Permissões**, endereço
`/dashboard/permissoes`) é um **catálogo somente leitura** de tudo o que o
sistema sabe controlar. Ela serve para você entender o que cada permissão faz e
quais planos a liberam. O subtítulo resume: *"Consulta read-only das permissões
do sistema. A liberação por plano acontece dentro de cada plano."*

> O que é uma "permissão" (capability)? É a autorização para fazer algo
> específico — por exemplo, "acessar o acervo completo" ou "gerenciar usuários".
> Cada permissão tem um nome amigável e um código técnico (mostrado em cinza,
> como `library.read`).

## As três seções da tela

As permissões aparecem agrupadas em três blocos, que você expande ou recolhe
clicando no título. Cada bloco mostra entre parênteses quantas permissões contém.

### 1. Editáveis no plano (azul)

São as permissões que **dependem do plano pago** do usuário (por exemplo, acesso
à biblioteca completa ou à Rede de Apoiadores). Para cada uma, a tela mostra
etiquetas com os planos que atualmente a liberam — clicar numa etiqueta abre o
plano correspondente.

Se uma permissão ainda **não está em nenhum plano**, aparece o aviso de que ela
não foi liberada e o atalho para abrir **Planos** e incluí-la.

Este bloco já vem **aberto** ao entrar na tela, porque é o único onde há decisão
a tomar.

### 2. Implícitas (todo logado tem) — o "plano base" (âmbar)

São as permissões do **plano base** (gratuito): tudo que faz parte de
simplesmente "ter uma conta". Exemplos: ver e editar o próprio perfil, ver perfis
públicos de outras pessoas, gerenciar a própria assinatura, aceitar convites e
sair de empresas, e o representante de PJ gerenciar os membros da própria
organização.

**Toda conta autenticada já recebe estas permissões automaticamente.** Por isso
elas não aparecem como opções nos planos pagos — não faria sentido cobrá-las.

### 3. Sistema (admin) (rosa)

São as permissões de **administração**, concedidas automaticamente a quem tem o
papel de **administrador**. Incluem gestão de usuários, organizações, assinaturas
e planos, gestão de permissões, cadastro de notícias, cursos, seminários,
eventos, biblioteca, templates de e-mail, triagem das mensagens de contato e
leitura do log de auditoria.

**Estas permissões nunca aparecem em planos** e não precisam de nenhuma
configuração: todo administrador já tem todas elas.

## Como se concede cada tipo de permissão

- **Por papel (administrador)** — automático. Quem é administrador tem todas as
  permissões de "Sistema". Para tornar alguém administrador, edite o usuário na
  tela **Usuários** e mude o campo **Papel** para "Administrador".
- **Pelo plano base** — automático para qualquer usuário logado (as "Implícitas").
- **Por plano pago** — é a única parte configurável: define-se dentro de cada
  plano quais permissões "Editáveis no plano" ele libera.

## Como editar as permissões de um plano

A tela de Permissões é só de consulta — **não se edita nada por aqui**. Para
liberar ou bloquear uma permissão para os assinantes:

1. Vá ao menu lateral **Planos** (`/dashboard/planos`).
2. Abra o plano desejado.
3. Marque ou desmarque as permissões que aquele plano deve conceder.
4. Salve. A mudança passa a valer para todos os assinantes daquele plano.

Atalhos prontos para essa tela estão espalhados pela tela de Permissões (links
"Planos" e as etiquetas de plano em cada permissão).

## Resumo

- Administradores têm acesso a tudo automaticamente (permissões de **Sistema**).
- Todo usuário logado já tem as permissões **Implícitas** do plano base.
- O que os demais usuários podem fazer além disso é definido pelo **plano** que
  assinaram — e isso se ajusta na tela **Planos**, não na de Permissões.

> Observação: a gestão de permissões é pensada para tela de computador. Em
> celular, a própria tela avisa para usar um monitor desktop.
