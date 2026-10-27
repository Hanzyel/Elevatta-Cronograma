# Publicação no GitHub Pages

## Pelo site do GitHub
1. Crie um novo repositório.
2. Faça upload de todos os arquivos deste pacote.
3. Abra **Settings > Pages**.
4. Em **Source**, selecione **Deploy from a branch**.
5. Selecione **main** e a pasta **/(root)**.
6. Clique em **Save**.

## Via Git
```bash
git init
git add .
git commit -m "Versão inicial do painel"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
git push -u origin main
```

Depois habilite GitHub Pages em **Settings > Pages**.
