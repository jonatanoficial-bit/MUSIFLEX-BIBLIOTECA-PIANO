# 🎹 MUSIFLEX — Biblioteca de Piano

Catálogo musical responsivo da Musiflex, nas cores **preto e laranja**, com o logotipo da escola.

## Como acessar

Após ativar o GitHub Pages em **Settings → Pages → Deploy from a branch → main → /(root)**, o site poderá ser acessado em:

**https://jonatanoficial-bit.github.io/MUSIFLEX-BIBLIOTECA-PIANO/**

O arquivo `index.html` já contém todo o CSS, JavaScript e o logo original incorporados. Portanto, não são necessárias instalações, servidores especiais nem build.

## Catálogo oficial incluído

Em 31/10/2026 o catálogo passou a conter **83 registros reais** (27 anteriores + **56 novos**) da planilha [MUSIFLEX — Catálogo Musical Oficial](https://docs.google.com/spreadsheets/d/13Nuht6S5lHq-giTlGrs84eG3MifpoCBUv-AvObDuGis/edit), preservando título, compositor, intérprete, tom, nível quando indicado, aba, páginas, material, BPM e outras observações. Todos foram adicionados ao aplicativo como **catálogo inicial**.

- Códigos estáveis `MFC-001` a `MFC-083`.
- Para visitantes novos, as 83 obras aparecem assim que abrem a página.
- Para quem já utiliza o catálogo, a nova versão **acrescenta os 56 novos registros** sem substituir registros locais existentes. Obras entre 001–027 excluídas manualmente não serão restauradas caso a importação anterior já tenha ocorrido.
- A atualização dos 56 registros ocorre uma única vez por navegador. Edições posteriores, exclusões e novos cadastros ficam somente naquele navegador até exportar/importar backup.
- Fonte editável para futuras migrações: `data/catalogo-inicial.json`.
- Sem vínculo vivo de sincronização: mudanças futuras no Google Sheets não aparecem automaticamente no GitHub.

## Atualização de 31/10/2026

A versão publicada foi atualizada com 56 novas músicas, chegando a 83 itens. Entraram repertórios populares (Queen, The Beatles, Guns N' Roses, Elton John), gospel, jazz/blues, cifras e obras eruditas. Registros duplicados no título, mas de seções físicas diferentes, permanecem separados. Alguns tipos estavam em branco na planilha original e são identificados como provisórios no campo Observações.

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
