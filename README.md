# Painel de Cronogramas de Obras

Aplicação web offline para planejamento semanal de obras, equipes, avanços, pendências, reprogramações e relatórios.

## Recursos
- Importação de planilhas semanais
- Histórico de planejamentos
- Pendências de semanas anteriores
- Cadastro de pessoas e equipes
- Relatório de equipes
- Avanço físico por atividade
- Controle de prazo e reprogramação
- Exportação/importação de backup JSON
- Compartilhamento de dados pelo celular/WhatsApp
- Layout responsivo para celular, tablet e desktop

## Como usar localmente
Abra o arquivo `index.html` no navegador.

## Publicar no GitHub Pages
1. Crie um repositório no GitHub.
2. Envie todos os arquivos deste pacote para a branch `main`.
3. Vá em **Settings > Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**.
5. Selecione `main` e `/ (root)`.
6. Salve.

O GitHub fornecerá um endereço semelhante a:

`https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`

## Dados
Os dados operacionais ficam armazenados localmente no navegador. Use **Exportar arquivo / Compartilhar dados** para transferir lançamentos entre dispositivos.

## Observação
O projeto foi preparado para funcionar como aplicação estática e não depende de servidor ou banco de dados para o uso básico.

## Publicação no Render

O projeto está pronto para hospedagem como **Render Static Site** e inclui `render.yaml`.

Configuração manual:
- Build Command: `echo "No build required"`
- Publish Directory: `.`
- Branch: `main`

Veja `DEPLOY_RENDER.md` para o passo a passo.
