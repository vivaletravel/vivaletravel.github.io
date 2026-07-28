# Vivale — site da marca

Site institucional da **Vivale** + a ferramenta **Guia da Mala** (consultora de mala virtual que capta leads).

> *viva o que vale*

---

## O que tem aqui

| Arquivo | O que é |
|---|---|
| `index.html` | Página inicial da marca (apresenta a Vivale e leva pro Guia da Mala). É a página que abre no endereço principal do site. |
| `guia-da-mala.html` | A ferramenta: a cliente responde algumas perguntas e recebe uma lista de mala personalizada em PDF. Capta nome, WhatsApp, destino e data. |
| `Vivale_Guia_da_Mala_LIGAR_NUVEM.txt` | Passo a passo pra ligar a nuvem (Google Sheets) e receber os cadastros das clientes numa planilha central. |
| `README.md` | Este arquivo. |

---

## Como publicar no GitHub Pages (grátis)

1. **Crie um repositório** no GitHub (ex.: `vivale-site`). Pode ser público.
2. **Suba os arquivos** deste pacote pra dentro do repositório (`index.html`, `guia-da-mala.html`, `.txt` e `README.md`). Dá pra arrastar e soltar na tela do GitHub em *Add file → Upload files*.
3. No repositório, vá em **Settings → Pages**.
4. Em *Build and deployment*, escolha **Deploy from a branch**, selecione a branch **main** e a pasta **/ (root)**. Salve.
5. Aguarde 1–2 minutos. O GitHub vai mostrar o endereço do site, algo como:
   `https://SEU-USUARIO.github.io/vivale-site/`
6. Pronto — a `index.html` abre nesse endereço, e o botão "Montar minha mala" leva pro `guia-da-mala.html`.

### Domínio próprio (opcional)
Se você tiver um domínio (ex.: `vivale.com.br`), em **Settings → Pages → Custom domain** é só informar o domínio e apontar o DNS conforme as instruções do GitHub. O GitHub cria um arquivo `CNAME` automaticamente.

---

## O que você precisa preencher antes de divulgar

### 1) WhatsApp da Vivale
- No arquivo **`guia-da-mala.html`**, lá no comecinho do script, ache:
  ```
  WHATSAPP_VIVALE: ""
  ```
  e coloque o número com DDD entre as aspas (ex.: `"5521999998888"`). Isso faz aparecer o botão "Chamar no WhatsApp" no resultado e o número no PDF.
- No arquivo **`index.html`**, procure e troque:
  - `https://wa.me/SEU_NUMERO_AQUI` → pelo seu número (ex.: `https://wa.me/5521999998888`)
  - `https://instagram.com/SEU_INSTAGRAM` → pelo @ real da Vivale

### 2) Senha do painel de leads
- No `guia-da-mala.html`, troque:
  ```
  PAINEL_SENHA: "vivale2026"
  ```
  pela senha que você quiser.

---

## O painel de leads (CRM)

- Acesse adicionando **`#painel`** no fim do endereço do Guia da Mala, ex.:
  `https://SEU-USUARIO.github.io/vivale-site/guia-da-mala.html#painel`
- Peça a senha (a que você definiu). **Só você deve usar esse endereço** — as clientes recebem o link normal, sem o `#painel`.
- No painel dá pra ver cada lead (destino, data, WhatsApp, perfil), mudar status (novo/contatado/fechado), anotar e exportar tudo em CSV.

### Receber os cadastros de qualquer aparelho
Como você vai mandar o link pras clientes preencherem sozinhas, os cadastros precisam cair numa planilha central na nuvem. O passo a passo está no arquivo **`Vivale_Guia_da_Mala_LIGAR_NUVEM.txt`** (leva ~10 min, é grátis, usa Google Sheets).

---

## Cuidado com dados (LGPD)

Você vai coletar nome, WhatsApp e dados de viagem de pessoas reais. Trate como dado pessoal: deixe claro pra cliente que ela está deixando os dados com a Vivale pra receber o guia e o contato, e não compartilhe a planilha com quem não precisa.
