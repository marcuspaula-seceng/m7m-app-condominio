# M7M — App do Condomínio (demonstração)

Protótipo navegável do app de condomínio da Villa M7M. Arquivo único, sem servidor,
sem banco e sem build: o `index.html` carrega tudo.

**É uma demonstração.** Os dados exibidos são fictícios e existem para mostrar o fluxo
das telas. Nenhum morador, unidade, contato ou valor real está neste repositório.

## Rodar localmente

Abra `index.html` no navegador. Não há passo de instalação.

## Publicação

Publicado via GitHub Pages a partir do branch `main`, raiz do repositório.

O site é servido com indexação bloqueada em duas camadas:

- `<meta name="robots" content="noindex,nofollow,noarchive,nosnippet,noimageindex">`
- `robots.txt` com `Disallow: /`

O `netlify.toml` e o `_headers` estão aqui de propósito, mas **não têm efeito no GitHub
Pages** — o Pages não permite definir cabeçalho HTTP. Eles só voltam a valer se a
hospedagem migrar para a Netlify, onde o `X-Robots-Tag` passa a ser aplicado na borda.

O `.nojekyll` existe porque o Jekyll ignora arquivos iniciados por `_`, e o `_headers`
some do deploy sem ele.

## Origem

Pacote gerado em `APP-NETLIFY-20260811-CLARO`. Este repositório é cópia validada por
SHA-256, não o original — o original permanece no acervo do EOS.

## Variante escura

Existe um pacote de tema escuro que **não** foi publicado: ele traz dois blocos `:root`
e dois `background` conflitantes, e renderiza claro com a barra do navegador escura.
Precisa de conserto antes de ir para qualquer lugar.
