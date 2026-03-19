# 🧾 Limpa Boleto

Uma ferramenta simples e eficiente para limpar códigos numéricos de boletos, removendo automaticamente pontos e espaços. Também permite a leitura por meio de imagens (requer chave de API do Google Vision).

🔗 **[Acessar ferramenta](https://willz1to.github.io/limpa-boleto)**

---

## ✨ Funcionalidades

- **Limpeza de texto** — cole o código do boleto e os pontos e espaços são removidos instantaneamente
- **Leitura de imagem** — capture a tela do boleto e extraia o código automaticamente via OCR
- **Validação automática** — verifica se o código resultante tem 44, 47 ou 48 dígitos (padrões válidos de boleto)
- **Cópia com um clique** — resultado pronto para colar onde precisar
- **Histórico de sessão** — acesso rápido aos últimos códigos processados
- **Sem instalação** — roda direto no navegador, sem servidores ou dados armazenados

---

## 🚀 Como usar

### Aba Texto
1. Copie o código do boleto (ex: `23792.11805 95181.000001 26002.854302 2 11560000090700`)
2. Cole no campo — o resultado aparece automaticamente
3. Clique no resultado para copiar

### Aba Imagem
1. Obtenha uma chave de API do Google Vision (veja instruções abaixo)
2. Cole a chave no campo 🔑 — ela será salva no seu navegador
3. Use **Win+Shift+S** para capturar a área do código no boleto e cole com **Ctrl+V**
4. Clique em **Ler imagem**

---

## 🔑 Como obter a chave do Google Vision (gratuita)

O Google Cloud Vision oferece **1.000 leituras gratuitas por mês** — mais que suficiente para uso pessoal.

1. Acesse [console.cloud.google.com](https://console.cloud.google.com) e crie uma conta
2. Crie um novo projeto (ex: "Limpa Boleto")
3. Vá em **APIs e serviços → Biblioteca**, pesquise **Cloud Vision API** e clique em **Ativar**
4. Vá em **APIs e serviços → Credenciais → Criar credenciais → Chave de API**
5. Copie a chave gerada (começa com `AIzaSy...`) e cole na ferramenta

> ⚠️ **Nunca compartilhe sua chave de API publicamente.** Ela fica salva apenas no seu próprio navegador e não é enviada para nenhum servidor além do Google.

---

## 🔒 Privacidade

Esta ferramenta funciona **100% no navegador**. Nenhum dado é enviado a servidores próprios. Ao usar a aba de imagem, a imagem é enviada diretamente ao Google Vision pela sua conexão — nenhum intermediário.

---

## 🛠️ Tecnologias

- HTML, CSS e JavaScript puros — sem frameworks ou dependências
- [Google Cloud Vision API](https://cloud.google.com/vision) para OCR de imagens

---

## 📄 Licença

MIT — livre para usar, modificar e distribuir.
