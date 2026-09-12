# Design

Os arquivos de origem do canvas do Claude Design ficam em `canvas/`.

Cada `.dc.html` é um artboard. `canvas.json` define a disposição deles.
Para alterar o canvas, editam-se esses arquivos e o canvas é gerado de novo a
partir deles — nunca se edita o HTML publicado diretamente.

- `Main.dc.html` — a página, largura de desktop
- `Mobile.dc.html` — a mesma página a 390px

## v0.1 — direção escolhida: ficha técnica

Fundo off-white quente (`#f7f5f1`), nome em Newsreader (serifada) sobre IBM Plex
Mono nos dados, foto colorida, campos em linhas de ficha, azul-tinta (`#3d5f8a`)
como único acento.

Descartada: uma direção "terminal" (fundo quase-preto, JetBrains Mono, foto em
preto e branco). Boa identidade, mas fecha a leitura para quem não é da área —
e esta página não é só profissional.
