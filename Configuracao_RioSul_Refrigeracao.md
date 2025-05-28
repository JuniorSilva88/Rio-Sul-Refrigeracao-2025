
# 🛠️ Documento Técnico – Configuração de Domínio, Site e E-mail Profissional  

**Domínio:** `riosulrefrigeracao.com.br`  
**Cliente:** Rio Sul Refrigeração  
**Data:** 28/05/2025  
**Responsável:** [Junior Silva](https://github.com/JuniorSilva88)

---

## 1. Configuração do Site no Netlify

- O site foi hospedado gratuitamente na plataforma **Netlify**.
- A aplicação principal está acessível por padrão no subdomínio:  
  `https://riosulrefrigeracao.netlify.app`
- Foi adicionado um **domínio personalizado** no painel do projeto:
  - `riosulrefrigeracao.com.br`
  - `www.riosulrefrigeracao.com.br`
- Ambos os domínios personalizados estão com **SSL/TLS automático (HTTPS)** ativado via Let’s Encrypt.

---

## 2. Configuração dos Servidores de Nome (DNS)

- O domínio `riosulrefrigeracao.com.br`, registrado no Registro.br, teve os servidores de DNS apontados para a **Netlify**:
  ```
  dns1.p09.nsone.net  
  dns2.p09.nsone.net  
  dns3.p09.nsone.net  
  dns4.p09.nsone.net
  ```
- A gestão completa dos registros DNS está sendo feita diretamente pelo painel da Netlify.

---

## 3. Configuração de E-mail Profissional com Umbler

- Para permitir o envio e recebimento de e-mails pela Umbler, foram criados os seguintes **registros MX**:

| Tipo | Nome | Valor                     | Prioridade | TTL   |
|------|------|---------------------------|------------|-------|
| MX   | @    | mx128.umbler.in.          | 10         | 3600  |
| MX   | @    | mx240.umbler.co.uk.       | 10         | 3600  |
| MX   | @    | mx364.umbler.com.         | 10         | 3600  |
| MX   | @    | mx783.umbler.com.br.      | 10         | 3600  |

- Adicionado também o **registro SPF** como **TXT**, permitindo que os servidores da Umbler enviem e-mails em nome do domínio:

| Tipo | Nome | Valor                                  | TTL   |
|------|------|-----------------------------------------|-------|
| TXT  | @    | v=spf1 include:spf.umbler.com ~all      | 3600  |

---

## 4. Testes e Propagação

- A propagação global de DNS pode levar até **48 horas**, mas geralmente ocorre em poucas horas.
- Após a propagação, o site estará disponível via domínio personalizado com HTTPS.
- O e-mail profissional estará apto para envio e recebimento com segurança (SPF ativo).

---

## 5. Considerações Finais

- Caso seja necessário aumentar a entregabilidade dos e-mails, recomenda-se futuramente configurar os registros **DKIM** e **DMARC** com a Umbler.
- A Umbler também oferece painel de gerenciamento de e-mails, redirecionamentos e aliases.
