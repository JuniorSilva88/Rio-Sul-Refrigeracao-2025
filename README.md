# 📘 Documentação / Documentation - Rio Sul Refrigeração

https://www.riosulrefrigeracao.com.br/

## 📌 Informações Gerais / General Information

- **Projeto / Project:** Site institucional para empresa de refrigeração / Institutional website for a refrigeration company.
- **Nome da empresa / Company Name:** Rio Sul Refrigeração
- **Objetivo / Purpose:** Apresentar os serviços oferecidos, facilitar o contato com clientes e fortalecer a presença online da marca.  
  To present the services offered, facilitate customer contact, and strengthen the company’s online presence.
- **Tecnologias utilizadas / Technologies Used:**
  - HTML5
  - CSS3
  - JavaScript
  - Bootstrap 5.3.3
  - Normalize.css
  - Google Fonts (Roboto Flex)
  - FormSubmit (para envio de formulários / for form submissions)

---

## 🌐 Estrutura de Arquivos / File Structure

├── index.html
├── sobre.html
├── servicos.html
├── contato.html
├── css/
│ ├── style.css
│ └── normalize.css
├── js/
│ └── current-year.js
├── img/
│ ├── logo-rs.png
│ ├── simbolo.jfif
│ ├── whatsapp.png
│ └── instagram.png

yaml
Copiar
Editar

---

## 🧩 Estrutura das Páginas / Page Structure

### `index.html` (Página Inicial / Home Page)

- Cabeçalho com logotipo e menu de navegação responsivo / Header with logo and responsive navigation menu  
- Seção principal com imagem e informações introdutórias / Main section with image and introductory information  
- Rodapé com redes sociais e contato / Footer with social media and contact info  

### `sobre.html` (Sobre / About)

- Informações institucionais / Company information  
- Texto sobre a empresa / Institutional text  
- Mapa do Google Maps incorporado / Embedded Google Map  

### `servicos.html` (Serviços / Services)

- Galeria de imagens / Image gallery  
- Efeito de zoom ao passar o mouse / Hover zoom effect  

### `contato.html` (Contato / Contact)

- Formulário com campos: Nome, E-mail, Telefone, Mensagem / Contact form with: Name, Email, Phone, Message  
- Envio com FormSubmit / Submission via FormSubmit  
- Resposta automática / Autoresponse  
- Imagem decorativa temática / Decorative refrigeration-themed image  

---

## 🎨 Paleta de Cores / Color Palette (`:root`)

- **Fundo / Background:** `#cbdad5`  
- **Hover:** `#89a7b1`  
- **Borda / Border:** `#566981`  
- **Sombra / Shadow:** `#3a415a`  
- **Fonte / Text Color:** `#34344e`  

---

## 🖌️ Estilização / Styling

- Reset CSS com Normalize / CSS reset with Normalize.css  
- Layout com Flexbox / Layout using Flexbox  
- Animações com `transition` e `transform: scale()` / Animations using `transition` and `transform: scale()`  
- Design responsivo com Bootstrap e media queries / Responsive design with Bootstrap and media queries  

---

## 📬 Formulário / Form

- Ação / Action: `https://formsubmit.co/alexandra_ale25@hotmail.com`  
- Resposta automática / Custom autoresponse  
- Validação HTML5 nos campos obrigatórios / Required fields with HTML5 validation  

---

## 🔧 Scripts

### `current-year.js`

```javascript
// Insere o ano atual no rodapé / Inserts the current year in the footer
const currentYear = new Date().getFullYear();
document.getElementById('current-year').textContent = currentYear;
👨‍💻 Desenvolvedor / Developer
Nome / Name: Junior Alexandre da Silva

GitHub: JuniorSilva88
