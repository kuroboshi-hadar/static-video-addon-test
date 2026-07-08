# JoJo Stone Ocean - Some-Stuffs Manual Stremio Addon

Addon estático pessoal para Stremio. Não precisa de Node, servidor, Real-Debrid ou banco de dados.

Ele cria um catálogo chamado `JoJo Some-Stuffs` com os episódios 01-38 de Stone Ocean. Cada episódio aponta manualmente para um batch da Some-Stuffs usando `infoHash + fileIdx`.

## Batches configurados

- Batch 01-12: `210187822a05188d56ac8e7f517680e3b08f800e`
- Batch 13-24: `77c1054d9e3b9b5363c5827a64aa521a92660b10`
- Batch 25-38: `64141a472c5a2db7c7abe58a4114cd76be467176`

Mapeamento usado:

- Ep 01-12: batch 01-12, `fileIdx = episódio - 1`
- Ep 13-24: batch 13-24, `fileIdx = episódio - 13`
- Ep 25-38: batch 25-38, `fileIdx = episódio - 25`

## Como publicar no GitHub Pages

1. Crie um repositório público no GitHub, por exemplo `jojo-somestuffs-stremio-addon`.
2. Suba todos estes arquivos na raiz do repositório. A raiz precisa conter `manifest.json`, `catalog/`, `meta/` e `stream/`.
3. No GitHub, vá em `Settings > Pages`.
4. Em `Build and deployment`, selecione `Deploy from a branch`.
5. Selecione `main` e `/root`.
6. Aguarde o GitHub Pages publicar.

A URL do manifest deve ficar assim:

```txt
https://SEU_USUARIO.github.io/NOME_DO_REPO/manifest.json
```

Instale essa URL no Stremio.

## Como usar no Stremio

1. Instale o addon pela URL do `manifest.json`.
2. Abra o catálogo `JoJo Some-Stuffs`.
3. Abra `JoJo’s Bizarre Adventure: Stone Ocean [Some-Stuffs]`.
4. Escolha o episódio 01-38.
5. Escolha o stream `Some-Stuffs BD 1080p`.

## Observação

Esse addon assume que dentro de cada torrent os arquivos de episódio estão em ordem crescente e sem arquivos de vídeo extras antes deles. Se algum batch tiver OP/ED/extra antes dos episódios na lista interna do torrent, o `fileIdx` daquele batch pode precisar de ajuste.
