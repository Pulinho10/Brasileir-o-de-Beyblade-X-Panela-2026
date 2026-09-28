# Panelão Brasileiro de Beyblade X 2026 — Registro de Partidas

Aplicação web estática para cadastro e homologação de partidas do torneio.

## Recursos
- Cadastro de jogadores com PIN de validação (armazenado como hash SHA-256 no navegador).
- Cadastro de juízes.
- Registro de fase, rodada, mesa/arena, placar, juiz e até 3 combos por jogador.
- Suporte a Lock Chip, Blade, Over Blade, Metal Blade, Assist Blade, Ratchet e Bit, com digitação livre.
- Validação independente de Jogador A e Jogador B.
- Partida considerada homologada apenas após as duas validações.
- Histórico pesquisável e filtro por status.
- Classificação calculada apenas com partidas homologadas.
- Backup JSON, importação JSON e exportação CSV.
- PWA/offline quando publicada via HTTPS (ex.: GitHub Pages).

## Uso local
Abra `index.html` em um navegador moderno. Para PWA/service worker, use um servidor HTTP local.

Exemplo com Python:

```bash
python -m http.server 8080
```

Depois acesse `http://localhost:8080`.

## Publicação no GitHub Pages
Envie estes arquivos para a raiz de um repositório e habilite **Settings → Pages → Deploy from a branch**.

## Armazenamento
Os dados ficam em `localStorage` do navegador/dispositivo. Faça backups JSON periódicos durante o evento.
