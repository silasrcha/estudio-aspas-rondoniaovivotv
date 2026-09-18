# Estúdio Aspas Rondoniaovivotv

Monta o card de citação do debate da Rondoniaovivotv sobre foto: cole o texto,
escolha a cor (azul, azul escuro ou branco), envie a foto e baixe o PNG.

É o Estúdio Aspas Debate enxugado: sem modelos geométricos, sem aspas, sem
editar nome/arroba. O cabeçalho é fixo — perfil do Marcos à esquerda,
"DEBATE / RONDONIAOVIVOTV" encostado à direita.

```bash
py -3 servidor.py        # http://localhost:8795
```

## Medidas

Vêm do Figma "DA Mídia — MR 2026", página "silas - edição", os três
TWEET-03-COM-LOGO (2430:1872 azul, 2431:1915 azul escuro, 2431:1934 branco).
Estão em auto-layout: Conteúdo com padding 35 / 67 / 41 / 72, gap 37 entre
cabeçalho e texto, card de 808 que cresce para baixo; a barra lateral é
absoluta e estica na proporção.

O card fica em Work Sans com entreletra de −4% no texto: sem isso a quebra de
linha sai diferente do Figma.

## Autossuficiente

Nenhuma chamada externa. Fontes do card e foto de perfil em base64 no
`index.html`; a Encode Sans da interface vem de `ativos/fontes/`.
