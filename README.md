<div align="center">

# 🔑 JWT Token API

API para geração de Tokens JWT e informações da conta.

![Status](https://img.shields.io/badge/Status-Online-green?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-GET-blue?style=for-the-badge)
![Region](https://img.shields.io/badge/Region-BR-yellow?style=for-the-badge)

API simples e rápida para desenvolvedores e vendedores que trabalham com bots e automações.

</div>

---

## ✨ Sobre

A **JWT Token API** fornece uma maneira simples e eficiente de gerar tokens JWT e obter informações da conta através de um único endpoint.

Ela é ideal para desenvolvedores e vendedores que utilizam bots, painéis ou outros sistemas automatizados.

---

## 🚀 Endpoint

```http
GET https://token-jwt-luiz.vercel.app/token
```

---

## 📥 Parâmetros

| Parâmetro | Tipo | Obrigatório | Descrição |
|------------|------|:----------:|------------|
| `uid` | String | ✅ | UID da conta |
| `password` | String | ✅ | Senha da conta |
| `key` | String | ✅ | Chave de acesso da API |

---

## 📖 Exemplo de requisição

```http
https://token-jwt-luiz.vercel.app/token?uid=123456789&password=minhasenha&key=lizin
```

---

## ✅ Resposta de sucesso

```json
{
  "access_token": "xxxxxxxxxxxxxxxx",
  "account_id": 15364885788,
  "account_name": "NomeDaConta",
  "open_id": "xxxxxxxxxxxxxxxx",
  "platform": 4,
  "region": "BR",
  "status": "success",
  "token": "eyJhbGciOi..."
}
```

---

## 📋 Campos retornados

| Campo | Descrição |
|---------|-----------|
| `access_token` | Token de acesso |
| `account_id` | ID da conta |
| `account_name` | Nick da conta |
| `open_id` | Identificador único |
| `platform` | Plataforma da conta |
| `region` | Região da conta |
| `status` | Status da requisição |
| `token` | Token JWT gerado |

---

## ❌ Possíveis erros

### Conta banida

```json
{
  "message": "Resposta OAuth sem access_token ou open_id"
}
```

Esse erro geralmente indica que a conta está banida ou indisponível.

---

## 🐍 Exemplo em Python

```python
import requests

url = "https://token-jwt-luiz.vercel.app/token"

params = {
    "uid": "123456789",
    "password": "minhasenha",
    "key": "lizin"
}

response = requests.get(url, params=params)

print(response.json())
```

---

## ⚡ Exemplo em JavaScript

```javascript
fetch("https://token-jwt-luiz.vercel.app/token?uid=123456789&password=minhasenha&key=lizin")
  .then(response => response.json())
  .then(data => console.log(data));
```

---

## 📜 Aviso

- A API é pública.
- O uso é livre.
- Se utilizar esta API em bots, painéis ou outros projetos, considere manter os créditos.
- Recomenda-se utilizar apenas contas próprias ou autorizadas.

---

## 📞 Suporte

[![Discord](https://img.shields.io/badge/Discord-@luizgustavo004431-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com)

[![Telegram](https://img.shields.io/badge/Telegram-@LuizvendasFF-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/LuizvendasFF)

[![WhatsApp](https://img.shields.io/badge/WhatsApp-+55%20(33)%2099963--3257-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/5533999633257)

---

<div align="center">

## ❤️ Desenvolvido por Luiz Gustavo

Se este projeto foi útil para você, considere deixar uma ⭐ no repositório.

</div>
