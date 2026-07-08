# JoJo Stone Ocean - Some-Stuffs Raw Picker

Addon estático do Stremio para os batches Some-Stuffs de Stone Ocean.

## O que tem aqui

- `JoJo Stone Ocean [Some-Stuffs] AUTO 01-38`: episódios 01-38; cada episódio tenta abrir o arquivo correto via `infoHash` + `fileIdx`.
- `RAW PICKER · Batch 01-12`, `13-24`, `25-38`: lista crua dos arquivos por `fileIdx`. Use isto se algum AUTO abrir errado.

## Como atualizar no GitHub Pages

Suba o conteúdo desta pasta na raiz do repo público e espere o GitHub Pages atualizar.
Depois reinstale o addon pelo manifest:

```txt
https://SEU_USUARIO.github.io/NOME_DO_REPO/manifest.json
```

## Observação

GitHub Pages é estático; ele não consegue baixar o magnet e rodar regex no arquivo `.torrent` na hora.
Por isso os nomes/índices estão pré-mapeados aqui.
