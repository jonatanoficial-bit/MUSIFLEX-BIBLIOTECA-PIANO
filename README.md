# 🎹 MUSIFLEX — Biblioteca de Piano

Catálogo musical responsivo da Musiflex, nas cores **preto e laranja**, com o logotipo da escola.

## Como acessar

Após ativar o GitHub Pages em **Settings → Pages → Deploy from a branch → main → /(root)**, o site poderá ser acessado em:

**https://jonatanoficial-bit.github.io/MUSIFLEX-BIBLIOTECA-PIANO/**

O arquivo `index.html` já contém todo o CSS, JavaScript e o logo original incorporados. Portanto, não são necessárias instalações, servidores especiais nem build.

## Catálogo oficial incluído

Atualizado em **03/11/2026** com **134 registros** da planilha [MUSIFLEX — Catálogo Musical Oficial](https://docs.google.com/spreadsheets/d/13Nuht6S5lHq-giTlGrs84eG3MifpoCBUv-AvObDuGis/edit).

- Versões: 27 registros iniciais → 83 (+56) → 95 (+12) → **134 (+39)**.
- Códigos `MFC-001` a `MFC-134`, sem duplicatas; a versão anterior foi preservada.
- Registros representam cada item físico, portanto uma mesma música pode ter cifra e partitura em abas diferentes.
- **Migração incremental não destrutiva**: quem já havia recebido os 95 registros recebe apenas os 39 novos. Registros editados ou excluídos intencionalmente no navegador não são restaurados nem sobrescritos.
- Visitantes novos encontram todos os 134 registros automaticamente.
- Campos como tom, artista, compositor, pasta, aba, página, cópias, BPM, compasso e observações são derivados da planilha sem inventar dados ausentes.
- Os dados versionados estão em `data/catalogo-inicial.json`. A planilha é a fonte das atualizações manuais, não há sincronização permanente.
- Novos cadastros realizados no navegador permanecem em `localStorage`. Faça backup JSON regular para evitar perdas.

## Atualização de 03/11/2026 — lote 4

Entraram 39 itens novos, incluindo músicas gospel (Laura Souguellis, Isaías Saad, Maria Marçal, Kirk Franklin), peças de piano clássico (Diabelli, Burgmüller, Tchaikovsky), pop/rock (Elton John, Lady Gaga, Van Halen, Billy Joel) e temas de cinema e séries (Star Wars, Stranger Things, Jurassic Park). Diferentes formatos das músicas **Your Song** e **Havana** foram preservados como itens distintos.

## Funcionalidades

- Cadastrar, editar e excluir estudos, partituras, cifras e partituras cifradas.
- Registrar título, compositor, intérprete/banda, tom, gênero, nível e observações.
- Localizar os documentos em arquivo físico por **pasta, aba/divisória e página**.
- Busca, filtros, favoritos, códigos de referência e impressão.
- Importar/Exportar **CSV** e fazer backup/restauração em **JSON**.
- Interface adaptável a computador, tablet e celular; funcionamento offline após acesso pelo site, quando o navegador oferece suporte ao service worker.

## ⚠️ Sobre os dados

Os cadastros ficam no **armazenamento local de cada navegador** (`localStorage`), não no repositório GitHub. Assim, o que for cadastrado em um celular não aparece automaticamente no computador. Para transferir registros: exporte backup JSON de um dispositivo e importe no outro.

**Faça backups periódicos.** Limpar dados do navegador pode apagar o catálogo. Para sincronização automática entre professores/dispositivos, uma futura versão deverá usar autenticação e banco de dados apropriados. Não coloque senhas nem tokens no código do site.

## Arquivos

- `index.html`: aplicativo completo com identidade visual e logotipo incorporados.
- `assets/musiflex-logo.png`: logo enviado pelo solicitante.
- `assets/musiflex-icon.svg`: ícone vetorial para atalho/instalação.
- `manifest.webmanifest`: configuração de aplicativo web.
- `sw.js`: cache básico para uso offline.
- `MODELO-IMPORTACAO.csv`: exemplo para cadastrar por planilha.
- `.nojekyll`: publicação de arquivos estáticos.

**Observação:** o campo Link abre PDFs hospedados externamente; o app não envia PDFs ao GitHub nem hospeda os arquivos de partitura.

Marca Musiflex utilizada como fornecida para a escola.
