# ATLAS 2.0 — Treino, HYROX e Nutrição

## Atualizar o app instalado no iPhone

1. **Antes de atualizar, abra o ATLAS antigo → Ajustes → Exportar JSON** e guarde o backup.
2. Descompacte o ZIP desta versão.
3. No repositório `atlas-gym` do GitHub, substitua **todos** os arquivos da raiz: `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png` e `README.md`.
4. Aguarde o GitHub Pages publicar a versão. Abra o mesmo endereço do app no Safari e recarregue.
5. O ATLAS 2.0 utiliza a **mesma chave local** (`atlas-gym-v1`) e migra os registros da versão 1.1 automaticamente se o endereço/origem e armazenamento do PWA forem preservados.
6. Se o Safari insistir na versão antiga, feche e reabra o app. Evite apagar o app ou limpar dados do site sem backup.

## Recursos

- Segunda: peito/costas; terça: HYROX; quarta: braços; quinta: HYROX; sexta: upper; sábado: pernas/ombros; domingo: descanso.
- Edição de dia, nome de treino, troca de dias, adição/edição/remoção e reordenação de exercícios.
- Editor em painel modal próprio para telas pequenas.
- Registro de carga/repetições/séries; gráfico de **carga máxima diária por exercício** na aba Histórico; atalho Ver evolução em cada exercício.
- Cronômetro, sessões HYROX, nutrição e metas, histórico e exportação/importação JSON.
- Identidade gym aesthetic preto e verde-lima com ícones premium fornecidos.

## Testes realizados

- `node --check` no JavaScript.
- Testes automatizados em Chromium (viewport iPhone 390 × 844) via Playwright: abrir Ajustes, adicionar e editar exercício, reordenar, selecionar dia, trocar dias, acessar gráfico, registrar sessão, registrar alimento e acionar exportação. Nenhum erro JavaScript durante os testes.
- **Não foi testado diretamente em Safari/iPhone físico nem publicado no GitHub automaticamente.** O cache offline/service worker só pode ser validado após publicação HTTPS.

## Armazenamento

O ATLAS usa localStorage. Dados não sincronizam entre dispositivos e podem ser perdidos ao apagar dados do site ou o app. Faça backups JSON frequentes. Metas nutricionais iniciais são exemplos, não prescrição.
