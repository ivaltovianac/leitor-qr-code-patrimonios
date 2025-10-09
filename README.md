# 📱 Sistema Leitor e Gerador de QR Code Patrimônio

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)]()
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?logo=javascript&logoColor=black)]()
[![Bootstrap 5](https://img.shields.io/badge/Bootstrap-5.0-7952B3?logo=bootstrap&logoColor=white)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

Sistema completo para **leitura, gerenciamento e geração de QR Codes patrimoniais**, com exportação para **Excel e PDF**.  
Projetado para facilitar o controle, a auditoria e a organização de bens patrimoniais com **tecnologia web moderna e responsiva**.

---

## 📚 Índice

- [📝 Descrição](#-descrição)
- [⚙️ Funcionalidades](#️-funcionalidades)
- [🧩 Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [💾 Instalação](#-instalação)
- [🚀 Uso](#-uso)
- [🖥️ Tela Principal](#️-tela-principal)
- [🔲 Gerador de QR Code](#-gerador-de-qr-code)
- [📤 Exportação de Dados](#-exportação-de-dados)
- [🔄 Uniformidade entre Scanner e Gerador de QR Code](#-uniformidade-entre-scanner-e-gerador-de-qr-code)
- [🤝 Contribuição](#-contribuição)
- [🪪 Licença](#-licença)
- [👨‍💻 Autor](#-autor)

---

## 📝 Descrição

Este sistema foi desenvolvido para **agilizar e dar precisão às auditorias patrimoniais**, utilizando QR Codes para identificar, controlar e rastrear bens.  
Além da leitura automática com dispositivos móveis ou câmeras integradas, o sistema permite **gerar QR Codes personalizados**, **filtrar e exportar dados**.  

📦 Feita para órgãos públicos, empresas e instituições que desejam modernizar e agilizar a sua **gestão patrimonial**.

---

## ⚙️ Funcionalidades

✅ **Scanner de QR Code** — leitura automática de informações patrimoniais.  
🧾 **Cadastro manual** — inclusão de patrimônios via formulário.  
🔍 **Filtros de busca avançados** — encontre bens facilmente.  
📑 **Exportação de dados** — gere relatórios em **Excel (.xlsx)** e **PDF**.  
🎨 **Gerador de QR Code customizado** — escolha cor, fundo e tamanho.  
💾 **Persistência local** — armazenamento no `localStorage`.  
📱 **Interface responsiva** — adaptável a dispositivos móveis.  
⚡ **PWA (Progressive Web App)** — acesso offline e instalação direta no navegador.  

---

## 🧩 Tecnologias Utilizadas

| Tecnologia | Função |
|-------------|--------|
| 🧱 **HTML5 / CSS3 / JavaScript (ES6+)** | Estrutura e lógica principal |
| 🎨 **Bootstrap 5** | Interface responsiva |
| 📷 **jsQR** | Leitura de QR Codes via câmera |
| 🧾 **QRCode.js** | Geração de QR Codes personalizados |
| 📊 **jsPDF + autotable** | Exportação de relatórios em PDF |
| 📈 **ExcelJS** | Exportação de planilhas Excel |
| 📸 **WebRTC API** | Acesso à câmera |
| ⚙️ **PWA (Service Worker + Manifest)** | Suporte offline |

---

## 💾 Instalação

1. **Clone este repositório**
   ```bash
   git clone https://github.com/ivaltovianac/leitor-qr-code-patrimonios.git
   ```

2. **Acesse a pasta do projeto**
   ```bash
   cd repositorio
   ```

3. **Abra o arquivo principal**
   - `index.html` → para usar o **scanner**
   - `gerador-qr-code.html` → para usar o **gerador**

> 💡 Nenhuma instalação de dependências é necessária — todas as bibliotecas são carregadas via **CDN**.

---

## 🚀 Uso

### 🔍 Scanner de QR Code
- Clique em **"Iniciar Scanner"** para ativar a câmera.  
- O sistema exibirá os dados automaticamente na tabela.  
- Use o campo de busca para filtrar resultados.  
- Exporte os dados para **Excel** ou **PDF**.  
- Clique em **"Parar Scanner"** para encerrar a leitura.  

### 🧾 Gerador de QR Code
- Preencha os campos com os dados do patrimônio.  
- Customize cor, tamanho e fundo.  
- Clique em **"Gerar QR Code"** para visualizar.  
- Baixe o QR Code em **PNG** clicando em **"Baixar PNG"**.  
- Clique em **"Limpar Campos"** para resetar o formulário.  

---

## 🖥️ Tela Principal

A interface principal é dividida em:

- 📸 **Scanner com visualização da câmera**.  
- 🧾 **Tabela paginada** com dados dos patrimônios.  
- 🔎 **Barra de ferramentas**: busca, limpar dados e exportação.  
- 🧩 **Formulário de adição manual** e modal de edição.  
- 🟢 **Indicador de status da câmera** (ativa/desativada).
---

### Leitor QR Code Patrimônios
<img width="1920" height="1797" alt="tela-principal-leitor-qr-code" src="https://github.com/user-attachments/assets/fcf216ed-c19d-46d1-b86b-c021aa14dd12" />

---
### Gerador de QR Code
<img width="1920" height="1933" alt="tela-gerador-de-qr-code" src="https://github.com/user-attachments/assets/581c339c-0c1a-4234-9cd1-80c8bf276ef7" />

---

## 📤 Exportação de Dados

📊 O sistema permite exportar facilmente os dados para:  

- **Excel (.xlsx)** — planilhas organizadas e formatadas.
  - ### Formato Excel
  <img width="1411" height="187" alt="image" src="https://github.com/user-attachments/assets/6c3f3ba4-3011-4f38-ac43-4665f5011c7a" /> 
- **PDF** — relatórios com tabelas e título personalizado.
  - Formato PDF:
  <img width="1900" height="874" alt="image" src="https://github.com/user-attachments/assets/82d7999a-c81c-4c2f-bf87-57d7c17eda67" /> 
  💡 Para a alteração da logo no PDF, mude no script.js na `const base64`.
---

## 🔄 Uniformidade entre Scanner e Gerador de QR Code

Para garantir que a leitura seja precisa, o QR Code deve seguir o formato abaixo:

```
Patrimônio:
Item:
Coordenação:
Servidor(a):
Coordenador:
```

💡 Esse modelo já vem pronto no campo de texto do gerador (`gerador-qr-code.html`), garantindo a compatibilidade total com o scanner.

---

## 🪪 Licença

📄 Este projeto está licenciado sob a [MIT License](LICENSE).  

---

## 👨‍💻 Autor
Desenvolvido por [**Ivalto Viana**](https://github.com/ivaltovianac).
