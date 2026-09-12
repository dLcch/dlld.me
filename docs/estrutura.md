# Estrutura do site

Mapa do que existe e do que está previsto. Cada seção nova entra aqui antes
de virar código.

## No ar

### Cabeçalho
Marca textual `dlld.me`. O slot de navegação existe no HTML, vazio,
esperando haver mais de uma seção para navegar.

### Perfil
Único bloco de conteúdo da v0.1.

- Foto
- Nome
- Apresentação (pai do Léo, marido da Fernanda, arquiteto de soluções com IA)
- Ficha: nascimento (1987), nacionalidade, origem, local

### Rodapé
- Versão da página (ex.: `v0.1`)
- "atualizada em {data}" — gerada automaticamente a partir do último commit
- `© {ano} Diego Domingues`

## Previsto

Nada definido ainda. Candidatos naturais conforme o site crescer:

- O que eu faço / serviços
- Stack e ferramentas
- Escritos
- Contato

## Infraestrutura

- Repositório: https://github.com/dLcch/dlld.me
- Publicação: GitHub Pages, origem "GitHub Actions" (necessária para a data
  automática do rodapé)
- Endereço provisório: https://dlcch.github.io/dlld.me/
- Domínio: dlld.me, registrado e com DNS na GoDaddy

### Pendência: verificação do domínio

O GitHub recusa `dlld.me` como domínio personalizado com a mensagem
"already taken" — outra conta reivindicou o domínio no passado, provavelmente
um dono anterior. A saída é a verificação de domínio em
github.com/settings/pages, que exige um registro TXT
`_github-pages-challenge-dlcch`. Depois de verificado, o domínio fica travado
para esta conta e ninguém mais consegue apontá-lo para outro site no GitHub.

DNS a configurar na GoDaddy:

| Tipo | Nome | Valor |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | dlcch.github.io |
| TXT | _github-pages-challenge-dlcch | (fornecido pelo GitHub) |

Os dois registros A do estacionamento da GoDaddy (76.223.105.230 e
13.248.243.5) precisam sair.

## Decisões tomadas

| Data | Decisão | Motivo |
|---|---|---|
| 2026-09-12 | Site estático sem build de framework | Zero manutenção, carrega instantâneo, nada pra quebrar |
| 2026-09-12 | Copy separada do HTML em `content/` | Reescrever texto sem caçar frase dentro de tag |
| 2026-09-12 | Ano de nascimento em vez de data completa | Data completa é dado usado em verificação de identidade |
| 2026-09-12 | Data do rodapé gerada pelo CI | Uma data escrita na mão vira mentira em duas semanas |
| 2026-09-12 | Direção visual: ficha técnica, não terminal escuro | A página não é só profissional; o visual não pode fechar a leitura |
| 2026-09-12 | Família na frase de apresentação, não na ficha | Gente numa linha de tabela vira inventário |
| 2026-09-12 | O site não tem molde: o critério é "vale ser público?" | Declarado na própria página, terceira linha da apresentação |
| 2026-09-12 | Caminhos de assets relativos, não absolutos | Absolutos quebram em qualquer endereço que não seja a raiz do domínio |
