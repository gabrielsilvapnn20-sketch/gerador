# Gerador de Stories

App web (um arquivo HTML, sem instalação) para montar sequências de stories do Instagram a partir de modelos com camadas e gerar as imagens em 1080x1920 PNG para cada influencer.

## Como usar

Abra `index.html` por um endereço https (por exemplo, GitHub Pages). No iPhone, abra no Safari e use Compartilhar → "Adicionar à Tela de Início".

- **Modelos:** crie sequências com fundo de foto ou imagem pronta, camadas de texto e imagem, referência semitransparente, áreas seguras e lugar do adesivo de link.
- **Gerar:** escolha o modelo, informe o nome (preenche `{nome}`), o link (`{link}`) e a foto. Ajuste cada story, prepare e compartilhe ou baixe (.zip).
- **Histórico:** registra o que foi gerado, para quem e quando.
- **Backup:** exporte/importe os modelos em `.json`. Os dados ficam no navegador (IndexedDB) de cada aparelho.

## Integração

O app expõe `window.GeradorStories` (`listarModelos`, `abrirGerar`, `gerar`, `listarHistorico`, `onExport`) para ser ligado a outro sistema.

`jszip.min.js` é o JSZip 3.10.1 (licença MIT), usado para gerar o .zip.
