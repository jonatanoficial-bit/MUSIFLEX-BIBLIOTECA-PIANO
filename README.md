# 🎹 MUSIFLEX — Biblioteca de Piano

Catálogo musical responsivo da Musiflex, nas cores **preto e laranja**, com o logotipo da escola.

## Como acessar

Após ativar o GitHub Pages em **Settings → Pages → Deploy from a branch → main → /(root)**, o site poderá ser acessado em:

**https://jonatanoficial-bit.github.io/MUSIFLEX-BIBLIOTECA-PIANO/**

O arquivo `index.html` já contém todo o CSS, JavaScript e o logo original incorporados. Portanto, não são necessárias instalações, servidores especiais nem build.

## Catálogo oficial incluído

Atualizado em 31/10/2026 com **95 registros** extraídos da planilha [MUSIFLEX — Catálogo Musical Oficial](https://docs.google.com/spreadsheets/d/13Nuht6S5lHq-giTlGrs84eG3MifpoCBUv-AvObDuGis/edit).

- Primeira versão: 27 registros; segunda: 83 registros (+56); terceira: **95 registros (+12)**.
- Códigos estáveis de `MFC-001` a `MFC-095`.
- Foram preservados os 83 registros anteriormente publicados; os 12 novos foram acrescentados.
- A identidade de uma obra considera título, aba **e artista** (exemplo: "O Sol", com artistas diferentes, é preservada em dois registros).
- O navegador com versão antiga recebe somente os registros novos pertinentes à sua migração. Edições e exclusões locais não são substituídas.
- Novos visitantes visualizam a coleção completa de 95 registros.
- Alguns campos não informados na planilha aparecem como não definidos, com observações explícitas.
- A fonte versionada dos dados fica em `data/catalogo-inicial.json`.
- **Não há sincronização automática**: os dados fornecidos via Google Sheets são importados em atualizações ao código; mudanças e novos cadastros locais são salvos em `localStorage`.

## Atualização de 31/10/2026 — lote 3

As novas entradas incluem Lady Gaga, Queen, Taylor Swift, Adele, Whitney Houston, Fernandinho, Gabriel Guedes, Get Worship e Marília Mendonça. A entrada "O Sol" de Vitor Kley é mantida separadamente de "O Sol" de Jota Quest. O registro 087 (De Quem É a Culpa) tem formato/aba incompletos na planilha e foi marcado como provisório.

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
