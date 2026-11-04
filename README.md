# 🎹 MUSIFLEX — Biblioteca de Piano

Catálogo musical responsivo da Musiflex, nas cores **preto e laranja**, com o logotipo da escola.

## Como acessar

Após ativar o GitHub Pages em **Settings → Pages → Deploy from a branch → main → /(root)**, o site poderá ser acessado em:

**https://jonatanoficial-bit.github.io/MUSIFLEX-BIBLIOTECA-PIANO/**

O arquivo `index.html` já contém todo o CSS, JavaScript e o logo original incorporados. Portanto, não são necessárias instalações, servidores especiais nem build.

## Catálogo oficial incluído

Atualizado em **04/11/2026** com **154 registros** da planilha [MUSIFLEX — Catálogo Musical Oficial](https://docs.google.com/spreadsheets/d/13Nuht6S5lHq-giTlGrs84eG3MifpoCBUv-AvObDuGis/edit).

- Histórico: 27 registros iniciais → 83 (+56) → 95 (+12) → 134 (+39) → **154 (+20)**.
- Códigos `MFC-001` a `MFC-154`, únicos. O conteúdo anterior foi preservado.
- **Migração incremental não destrutiva**: navegadores que já receberam 134 registros recebem apenas os 20 novos. Edições/exclusões anteriores no navegador não são revertidas.
- Identificação de versões: título, aba, artista, **tipo de material e tom**. Isso preserva cifras de uma mesma música em tonalidades diferentes (ex.: `Tattooed Heart` em Dó e Sol maior), bem como partituras e cifras da mesma obra.
- Novos visitantes recebem as 154 obras. O código principal inclui os registros sem necessitar de conexão direta com Google Sheets.
- Os dados de origem ficam também em `data/catalogo-inicial.json`, para conferência e próximas migrações.
- A planilha é consultada em atualizações manuais; **não existe sincronização contínua automática** com Google Sheets.
- Cadastro realizado diretamente no site é salvo por navegador em `localStorage`. Faça backups JSON regularmente.

## Atualização de 04/11/2026 — lote 5

Foram incorporadas 20 entradas entre `MFC-135` e `MFC-154`: repertório de Adele, John Legend, Michael Jackson, Ariana Grande, Bruno Mars, The Weeknd, Elis Regina e RPM; gospel de Renascer Praise, Eli Soares, Hillsong, Sued Silva e Isaías Saad; além de estudos de música popular. Foram preservadas as versões distintas de `Bondade de Deus`, `All of Me`, `Hakuna Matata`, `When I Was Your Man` e `Tattooed Heart`.

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
