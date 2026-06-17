JWT Token API

API para geração de tokens JWT e informações básicas da conta.

✨ Descrição

A JWT Token API foi desenvolvida para fornecer uma forma simples e rápida de gerar tokens JWT e obter informações da conta. Ela é especialmente útil para desenvolvedores e vendedores que trabalham com bots, sistemas automatizados e integrações que necessitam de autenticação e dados da conta.

---

📌 Endpoint

GET https://token-jwt-luiz.vercel.app/token

---

📥 Parâmetros

Parâmetro| Tipo| Obrigatório| Descrição
"uid"| String| ✅| UID da conta
"password"| String| ✅| Senha da conta
"key"| String| ✅| Chave de acesso da API

Exemplo

https://token-jwt-luiz.vercel.app/token?uid=123456789&password=minhasenha&key=lizin

---

✅ Resposta de sucesso

{
  "access_token": "xxxxxxxxxxxxxxxxxxxxxxxx",
  "account_id": 15364885788,
  "account_name": "NomeDaConta",
  "open_id": "xxxxxxxxxxxxxxxx",
  "platform": 4,
  "region": "BR",
  "status": "success",
  "token": "eyJhbGciOi..."
}

Campos retornados

Campo| Descrição
"access_token"| Token de acesso
"account_id"| ID da conta
"account_name"| Nick da conta
"open_id"| Identificador único
"platform"| Plataforma da conta
"region"| Região da conta
"status"| Status da requisição
"token"| Token JWT gerado

---

❌ Resposta de erro

Conta banida

{
  "message": "Resposta OAuth sem access_token ou open_id"
}

Essa resposta indica que a conta provavelmente está banida ou indisponível.

---

📖 Exemplo em Python

import requests

url = "https://token-jwt-luiz.vercel.app/token"

params = {
    "uid": "123456789",
    "password": "minhasenha",
    "key": "lizin"
}

response = requests.get(url, params=params)

print(response.json())

---

📖 Exemplo em JavaScript

fetch("https://token-jwt-luiz.vercel.app/token?uid=123456789&password=minhasenha&key=lizin")
  .then(response => response.json())
  .then(data => console.log(data));

---

⚠️ Aviso

- A API é pública e pode ser utilizada livremente.
- Se utilizar esta API em bots, painéis ou outros projetos, mantenha os créditos.
- Recomenda-se utilizá-la apenas em contas próprias ou autorizadas.

---

❤️ Créditos

Desenvolvido por Luiz Gustavo

Discord

@luizgustavo004431

Telegram

@LuizvendasFF

WhatsApp

+55 (33) 99963-3257
