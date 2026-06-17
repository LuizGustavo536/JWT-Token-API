<div align="center">JWT Token API

API para geração de tokens JWT e informações da conta.

"Status" (https://img.shields.io/badge/status-online-green)
"Method" (https://img.shields.io/badge/method-GET-blue)
"Region" (https://img.shields.io/badge/region-BR-yellow)

</div>---

✨ Sobre

A JWT Token API foi criada para fornecer uma maneira simples e rápida de gerar tokens JWT e obter informações da conta.

Ideal para desenvolvedores e vendedores que trabalham com bots e automações, oferecendo uma integração simples através de um único endpoint.

---

🚀 Endpoint

GET https://token-jwt-luiz.vercel.app/token

---

📥 Parâmetros

Parâmetro| Obrigatório| Descrição
uid| ✅| UID da conta
password| ✅| Senha da conta
key| ✅| Chave de acesso da API

---

📖 Exemplo

https://token-jwt-luiz.vercel.app/token?uid=123456789&password=minhasenha&key=lizin

---

✅ Resposta

{
  "access_token": "...",
  "account_id": 15364885788,
  "account_name": "NomeDaConta",
  "open_id": "...",
  "platform": 4,
  "region": "BR",
  "status": "success",
  "token": "eyJhbGciOi..."
}

---

❌ Erros

Conta banida

{
  "message": "Resposta OAuth sem access_token ou open_id"
}

---

💖 Apoie o Projeto

Se esta API for útil para você, considere dar os créditos ao autor.

<div align="center">""Discord" (https://img.shields.io/badge/Discord-@luizgustavo004431-5865F2?style=for-the-badge&logo=discord&logoColor=white)" (https://discord.com)

""Telegram" (https://img.shields.io/badge/Telegram-@LuizvendasFF-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)" (https://t.me/LuizvendasFF)

""WhatsApp" (https://img.shields.io/badge/WhatsApp-Contato-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)" (https://wa.me/5533999633257)

</div>---

<div align="center">Desenvolvido por Luiz Gustavo

⭐ Se gostou do projeto, considere deixar uma estrela no repositório.

</div>
