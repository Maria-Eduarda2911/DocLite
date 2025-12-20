# ⚡ DocLite 

> **Visualizador universal de arquivos 100% offline, seguro e leve.**

**DocuLite** é uma ferramenta de *arquivo único* que permite abrir, visualizar e analisar planilhas e documentos diretamente no navegador, sem enviar nada para nenhum servidor.

[![Assista ao Vídeo de Demonstração](https://img.youtube.com/vi/sicFI6fTIcs/maxresdefault.jpg)](https://youtu.be/sicFI6fTIcs)
> *Clique na imagem acima para ver o vídeo de demonstração.*
![Tela Principal](/prints/8b76e80c-3476-4fdb-a5e0-f83256ad7a39.jpg)

---

## 🎯 Propósito e Usabilidade

O projeto nasceu da necessidade de visualizar arquivos pesados ou de formatos variados rapidamente, sem depender de softwares proprietários (como Office) ou conversores online que comprometem a privacidade dos dados.

### Destaques de Usabilidade:
* **Histórico Persistente:** Graças ao **IndexedDB**, seus arquivos ficam salvos dentro do navegador. Você pode fechar a aba e voltar depois, e o arquivo abrirá instantaneamente sem alertas de segurança irritantes.
* **Leitura Confortável:** Documentos (PDF/DOCX) são renderizados em um layout de "folha de papel" com sombreamento, alinhamento centralizado e zoom otimizado.
* **Seleção de Texto Nativa:** Copie textos de PDFs e arquivos DOCX sem quebra de formatação ou blocos visuais estranhos.
* **Feedback Visual:** O sistema notifica quando um texto é copiado ou quando um arquivo está sendo processado.

---

## 🚀 Principais Funcionalidades

### 1. Análise de Dados (CSV e Excel)
Transforma arquivos brutos em tabelas interativas e modernas.
* **Processamento Inteligente:** Detecta automaticamente colunas de **Moeda** (alinhadas à direita, cor verde), **Datas** (converte números de série do Excel, ex: `45929` para `15/09/2025`) e **Texto**.
* **Modo Grade (Grid):** Opção para visualizar os dados como no Excel clássico.
* **Filtros Avançados:** Filtre por coluna ou use a busca global.

![Visualização em Tabela](/prints/{D3642435-A0ED-48E5-B625-C5FEBE12CF6C}.png)

### 2. Visualizador de Documentos (PDF e Word)
Renderização fiel de documentos de texto.
* **PDF:** Renderização via Canvas com uma camada de texto transparente para seleção precisa.
* **DOCX:** Conversão limpa para HTML, mantendo a estrutura de parágrafos e títulos.

![Visualizador PDF](/prints/f600fb7b-3b79-4601-9f44-1a1ed0fe7945.jpg)
![Visualizador DOCX](/prints/ed1cbe1c-df65-44f3-9bc8-da4ebed8bae8.jpg)

### 3. Ferramentas de Produtividade
* **Modal de Detalhes:** Clique em qualquer linha da tabela para ver os dados em cartões organizados. Links (HTTP/HTTPS) tornam-se botões clicáveis automaticamente.
* **Busca Rápida:** Barra de pesquisa otimizada no cabeçalho.

![Modal de Detalhes](/prints/{FFCDC16B-911B-464F-BD4E-DA36749A4E02}.png)
![Links no Modal](/prints/{86CB511B-C368-4F4F-B000-E819FDF33444}.png)

---

## 🛠️ Como foi feito (Tecnologia)

O DocuLite foi construído com a filosofia **Zero-Backend**. Toda a lógica reside em um único arquivo HTML contendo CSS e JS minificados para máxima performance.

### Tecnologias:
* **Core:** HTML5, CSS3 (com CSS Variables), Vanilla JavaScript (ES6+).
* **Armazenamento:** `IndexedDB` (Banco de dados NoSQL dentro do navegador) para cache de arquivos grandes.
* **Ícones:** Lucide Icons.

### Bibliotecas de Processamento:
* `PapaParse`: Para análise ultra-rápida de CSV.
* `SheetJS (XLSX)`: Para leitura e conversão de planilhas Excel.
* `Mammoth.js`: Para converter .docx em HTML limpo.
* `PDF.js`: Tecnologia da Mozilla para renderizar PDFs com precisão.

---

## 📦 Como Usar

1.  Baixe o arquivo `DocLite.html`.
2.  Abra em qualquer navegador moderno (Chrome, Edge, Firefox, Brave).
3.  Arraste um arquivo ou clique em **Importar**.
4.  Seus arquivos recentes aparecerão na barra lateral automaticamente.

### Formatos Suportados
| Tipo | Extensões |
| :--- | :--- |
| Planilhas | `.csv`, `.xlsx`, `.xls` |
| Documentos | `.docx`, `.doc`, `.pdf` |
| Dados/Texto | `.json`, `.txt` |

---

*Desenvolvido por Maria Eduarda.*
