# dlld.me

Site pessoal de Diego Domingues.

## Como isso funciona

O que está na raiz é publicado. O que está em `content/`, `media/`, `design/` e `docs/` é matéria-prima e não vai pro ar.

```
index.html      a página publicada
CNAME           amarra o domínio dlld.me ao GitHub Pages
assets/         css, imagens otimizadas e fontes que a página carrega
content/        a copy em markdown — fonte da verdade dos textos
media/          originais (fotos em alta, etc). Não versionado.
design/         canvas do Claude Design e referências visuais
docs/           changelog, mapa de estrutura, briefing de branding
```

## Publicação

Todo push na branch `main` dispara o workflow `.github/workflows/deploy.yml`,
que injeta a data do último commit no rodapé e publica no GitHub Pages.

Não edite a data do rodapé na mão — ela é gerada.

## Ao mudar de versão

1. Atualize `docs/CHANGELOG.md`
2. Atualize o número da versão no rodapé do `index.html`
3. Commit e push
