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
