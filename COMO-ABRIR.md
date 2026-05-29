# Como abrir o Manual do Administrador

O manual é um site estático (HTML) com busca embutida. Por usar carregamento dinâmico das páginas,
ele precisa ser **servido por um servidor local** (abrir o `index.html` direto pelo navegador, via
`file://`, não funciona para a busca/navegação).

## Opção 1 — com Node.js instalado (recomendado)

Abra um terminal nesta pasta (`admin-portal`) e rode:

```bash
npx --yes serve .
```

Depois abra o endereço que aparecer (algo como `http://localhost:3000`).

## Opção 2 — com Python instalado

```bash
python -m http.server 8080
```

E abra `http://localhost:8080`.

## Opção 3 — hospedar

Suba o conteúdo desta pasta em qualquer hospedagem de site estático (ex.: o mesmo servidor do site,
um bucket, ou um serviço de páginas). Tudo é estático e funciona offline (os arquivos do Docsify estão
em `vendor/`, sem depender de internet).

> O conteúdo em si são os arquivos `.md` em `secoes/` — legíveis em qualquer editor de texto, mesmo sem
> abrir o site.
