# Publicar no Render (onrender.com)

Este projeto é um site estático (HTML/CSS/JS) e deve ser publicado no Render como **Static Site**.

## Opção 1 — Static Site (mais simples)

1. Envie todos os arquivos deste pacote para um repositório no GitHub.
2. Acesse o Dashboard do Render.
3. Clique em **New +** → **Static Site**.
4. Conecte sua conta do GitHub e selecione o repositório.
5. Configure:
   - **Name:** `painel-cronogramas-obras` (ou outro nome disponível)
   - **Branch:** `main`
   - **Build Command:** `echo "No build required"`
   - **Publish Directory:** `.`
6. Clique em **Create Static Site**.
7. Quando o deploy terminar, o endereço será parecido com:
   `https://painel-cronogramas-obras.onrender.com`

## Opção 2 — Blueprint com render.yaml

O pacote já contém `render.yaml`.

1. Suba o repositório para o GitHub.
2. No Render, crie um novo **Blueprint**.
3. Selecione o repositório.
4. O Render lerá o `render.yaml` e criará o Static Site.

## Atualizações futuras

Com `autoDeployTrigger: commit`, toda alteração enviada para a branch conectada do GitHub pode gerar um novo deploy automaticamente.

## Dados do painel

Os lançamentos do painel continuam armazenados no navegador (`localStorage`). Eles não ficam gravados no servidor do Render. Use **Compartilhar dados / Exportar arquivo** para transferir os dados entre celular e computador.


## Correção para acesso no celular
No Render, em **Redirects/Rewrites**, adicione: Source `/*`, Destination `/index.html`, Action `Rewrite`. Isso evita `Not Found` ao abrir atalhos/PWA ou links com caminhos antigos. Depois faça um novo deploy e, no celular, remova o atalho/PWA antigo e abra novamente a URL raiz.
