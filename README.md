<div align="center">

<!-- BANNER -->
<img src="https://raw.githubusercontent.com/zenomdevs/uploads/main/049njw.jpeg" width="120" style="border-radius:20px;" />

<br/>

# 🧩 WAGURI API's 🎨

**Uma plataforma completa de APIs**  
**para desenvolvedores que criam sistemas modernos e automatizados.**

<br/>

[![Status](https://img.shields.io/badge/Status-Online%20✓-22c55e?style=for-the-badge&labelColor=0d1117&color=22c55e)](https://waguapis.online)  
[![Endpoints](https://img.shields.io/badge/Endpoints-80%2B-8b5cf6?style=for-the-badge&labelColor=0d1117)](https://waguapis.online)  
[![Uptime](https://img.shields.io/badge/Uptime-99.9%25-22c55e?style=for-the-badge&labelColor=0d1117)](https://waguapis.online)  
[![Resposta](https://img.shields.io/badge/Resposta-menor_que_2s-8b5cf6?style=for-the-badge&labelColor=0d1117)](https://waguapis.online)  
[![Lançamento](https://img.shields.io/badge/Lançamento-2026-ec4899?style=for-the-badge&labelColor=0d1117)](https://waguapis.online)  

<br/>

<a href="https://waguapis.online">
  <img src="https://img.shields.io/badge/%F0%9F%9A%80%20Acessar%20Plataforma-waguapis.online-8b5cf6?style=for-the-badge&labelColor=1a0a2e&color=8b5cf6" height="42" />
</a>
&nbsp;&nbsp;
<a href="https://instagram.com/uzuback">
  <img src="https://img.shields.io/badge/%F0%9F%93%B8%20Instagram-uzuback-ec4899?style=for-the-badge&labelColor=1a0a2e&color=ec4899" height="42" />
</a>

</div>

---

## 📋 Índice

- [🟣 Sobre a plataforma](#-sobre-a-plataforma)
- [⚡ Recursos disponíveis](#-recursos-disponíveis)
- [🔑 Como adquirir seu Token](#-como-adquirir-seu-token)
- [📦 Planos](#-planos)
- [🌐 Base URL](#-base-url)
- [📡 Endpoints documentados](#-endpoints-documentados)
- [🔍 YouTube Search](#-youtube-search)
- [🎴 Sticker / Figurinha](#-sticker--figurinha)
- [⬇️ Downloader Universal](#️-downloader-universal)
- [🛠️ Ferramentas de integração](#️-ferramentas-de-integração)
- [❌ Erros comuns](#-erros-comuns)
- [👨‍💻 Criador](#-criador)
- [📄 Licença](#-licença)

---

## 🟣 Sobre a plataforma

A **WAGURI API's** é uma plataforma premium desenvolvida para desenvolvedores que precisam de ferramentas confiáveis, rápidas e modernas para criar bots, sistemas automatizados, websites e aplicações.

Com mais de **80 endpoints** ativos, a plataforma oferece desde buscas e downloads de mídia até criação de figurinhas, canvas customizáveis e uploads em nuvem — tudo via simples requisições HTTP.

```
✅ Sem necessidade de configurações complexas
✅ Resposta JSON limpa e organizada
✅ Compatível com Node.js, Python, PHP e qualquer linguagem HTTP
✅ Infraestrutura estável com uptime de 99.9%
✅ Atualizações constantes com novos endpoints
```

---

## ⚡ Recursos disponíveis

| Recurso | Descrição |
|--------|-----------|
| 🔑 **Key Premium** | Acesso completo a todos os endpoints com suporte dedicado |
| 📡 **APIs Premium** | 80+ endpoints: buscas, consultas, automações, mídias e mais |
| 🎨 **Canvas Code** | Geração de banners, cards e artes via código puro, sem módulos externos |
| ☁️ **Upload de Mídias** | Envio de imagens, vídeos e arquivos com retorno de link imediato |
| ⬇️ **Downloader Universal** | Download de vídeos do YouTube, Instagram, TikTok e outros |
| 🎴 **Stickers e Figurinhas** | Criação de figurinhas WebP estáticas e animadas para WhatsApp |
| ⚙️ **Ferramentas Extras** | Geradores, consultas, automações e utilitários variados |
| 🔗 **Integração Fácil** | HTTP simples, documentação clara, parâmetros detalhados |
| ⚡ **Alta Performance** | Servidores rápidos, resposta em menos de 2 segundos |

---

## 🔑 Como adquirir seu Token

> ⚠️ **O parâmetro `apitoken` é obrigatório em todas as rotas.** Sem ele, a API retorna `401 Unauthorized`.

Siga os passos abaixo para obter sua chave de acesso:

```
Passo 1 → Entre na aba principal da api e clique em comprar key
Passo 2 → Escolha o plano que melhor atende seu projeto
Passo 3 → Após a confirmação, receba seu apitoken na hora
Passo 4 → Use ?apitoken=SUA_KEY em qualquer endpoint
```

**Exemplo de uso do token numa requisição:**

```
GET https://waguapis.online/yt-search?titulo=matuê+1993&apitoken=SUA_KEY
```

---

## 📦 Planos

| Plano | Requisições | Endpoints | Suporte | Preço |
|-------|-------------|-----------|---------|-------|
| **Básico** | 1000 | Todos | Instagram | 1R$ |
| **Premium** | 5000 | Todos | Instagram | 5R$ |
| **Enterprise** | 2000 | Todos | Instagram | 20R$ |

> 📲 Para contratar, acesse: **[instagram.com/uzuback](https://instagram.com/uzuback/links)**

---

## 🌐 Base URL

```
https://waguapis.online
```

Todas as rotas são acessadas via `GET` e retornam `application/json`.

---

## 📡 Endpoints documentados

### 🔍 YouTube Search

Busca vídeos no YouTube e retorna informações completas sobre o resultado mais relevante.

**Rota:**
```
GET /yt-search
```

**Parâmetros:**

| Parâmetro | Tipo | Status | Descrição |
|-----------|------|--------|-----------|
| `titulo` | string | ✅ obrigatório | Nome do vídeo ou música |
| `apitoken` | string | ✅ obrigatório | Sua chave de acesso |

**Exemplo de URL:**
```
https://waguapis.online/yt-search?titulo=matuê%201993&apitoken=SUA_KEY
```

<details>
<summary>📦 <strong>Fetch (JavaScript)</strong></summary>

```javascript
const response = await fetch(
  'https://waguapis.online/yt-search?titulo=matuê+1993&apitoken=SUA_KEY'
);

const data = await response.json();
console.log(data);
```

</details>

<details>
<summary>📦 <strong>Axios (Node.js)</strong></summary>

```javascript
const axios = require('axios');

const { data } = await axios.get('https://waguapis.online/yt-search', {
  params: {
    titulo: 'matuê 1993',
    apitoken: 'SUA_KEY'
  }
});

console.log(data);
```

</details>

<details>
<summary>📦 <strong>cURL (Terminal)</strong></summary>

```bash
curl -X GET \
  "https://waguapis.online/yt-search?titulo=matuê%201993&apitoken=SUA_KEY" \
  -H "Content-Type: application/json"
```

</details>

<details>
<summary>📦 <strong>Request (Node.js)</strong></summary>

```javascript
const request = require('request');

request.get({
  url: 'https://waguapis.online/yt-search',
  qs: {
    titulo: 'matuê 1993',
    apitoken: 'SUA_KEY'
  },
  json: true
}, (err, res, body) => {
  console.log(body);
});
```

</details>

**Retorno JSON (`200 OK`):**

```json
{
  "resxz": {
    "type": "video",
    "videoId": "gyVmdwtvKwg",
    "url": "https://youtube.com/watch?v=gyVmdwtvKwg",
    "title": "Matuê - 1993",
    "description": "333: SALVE TODOS.",
    "image": "https://i.ytimg.com/vi/gyVmdwtvKwg/hq720.jpg",
    "thumbnail": "https://i.ytimg.com/vi/gyVmdwtvKwg/hq720.jpg",
    "seconds": 126,
    "timestamp": "2:06",
    "duration": {
      "seconds": 126,
      "timestamp": "2:06"
    },
    "ago": "1 year ago",
    "views": 32127829,
    "author": {
      "name": "30PRAUM",
      "url": "https://youtube.com/@30PRAUM"
    }
  }
}
```

---

### 🎴 Sticker / Figurinha

Converte imagens ou vídeos em figurinhas WebP para WhatsApp (estáticas ou animadas).

**Rota:**
```
GET /sticker
```

**Parâmetros:**

| Parâmetro | Tipo | Status | Descrição |
|-----------|------|--------|-----------|
| `url` | string | ✅ obrigatório | URL da imagem ou vídeo |
| `pack` | string | ⬜ opcional | Nome do pacote de figurinhas |
| `author` | string | ⬜ opcional | Autor da figurinha |
| `apitoken` | string | ✅ obrigatório | Sua chave de acesso |

**Exemplo de URL:**
```
https://waguapis.online/sticker?url=https://exemplo.com/img.png&pack=Meu%20Pack&author=WAGURI&apitoken=SUA_KEY
```

<details>
<summary>📦 <strong>Fetch (JavaScript)</strong></summary>

```javascript
const params = new URLSearchParams({
  url: 'https://exemplo.com/imagem.png',
  pack: 'Meu Pack',
  author: 'WAGURI',
  apitoken: 'SUA_KEY'
});

const res = await fetch(`https://waguapis.online/sticker?${params}`);
const data = await res.json();
console.log(data.sticker); // URL do WebP gerado
```

</details>

<details>
<summary>📦 <strong>Axios (Node.js)</strong></summary>

```javascript
const { data } = await axios.get('https://waguapis.online/sticker', {
  params: {
    url: 'https://exemplo.com/imagem.png',
    pack: 'Meu Pack',
    author: 'WAGURI',
    apitoken: 'SUA_KEY'
  }
});

console.log(data);
```

</details>

<details>
<summary>📦 <strong>cURL (Terminal)</strong></summary>

```bash
curl -X GET \
  "https://waguapis.online/sticker?url=https://exemplo.com/imagem.png&pack=Meu%20Pack&author=WAGURI&apitoken=SUA_KEY"
```

</details>

<details>
<summary>📦 <strong>Request (Node.js)</strong></summary>

```javascript
request.get({
  url: 'https://waguapis.online/sticker',
  qs: {
    url: 'https://exemplo.com/imagem.png',
    pack: 'Meu Pack',
    author: 'WAGURI',
    apitoken: 'SUA_KEY'
  },
  json: true
}, (err, res, body) => console.log(body));
```

</details>

**Retorno JSON (`200 OK`):**

```json
{
  "status": true,
  "sticker": "https://waguapis.online/cdn/stickers/abc123.webp",
  "pack": "Meu Pack",
  "author": "WAGURI",
  "format": "webp"
}
```

---

### ⬇️ Downloader Universal

Faz o download de vídeos das principais plataformas (YouTube, Instagram, TikTok e mais) a partir de um link.

**Rota:**
```
GET /download
```

**Parâmetros:**

| Parâmetro | Tipo | Status | Descrição |
|-----------|------|--------|-----------|
| `url` | string | ✅ obrigatório | Link do vídeo a baixar |
| `quality` | string | ⬜ opcional | `360p` / `720p` / `1080p` |
| `apitoken` | string | ✅ obrigatório | Sua chave de acesso |

**Exemplo de URL:**
```
https://waguapis.online/download?url=https://youtu.be/dQw4w9WgXcQ&quality=720p&apitoken=SUA_KEY
```

<details>
<summary>📦 <strong>Fetch (JavaScript)</strong></summary>

```javascript
const res = await fetch(
  'https://waguapis.online/download?url=https://youtu.be/dQw4w9WgXcQ&quality=720p&apitoken=SUA_KEY'
);

const data = await res.json();
console.log(data.download_url);
```

</details>

<details>
<summary>📦 <strong>Axios (Node.js)</strong></summary>

```javascript
const { data } = await axios.get('https://waguapis.online/download', {
  params: {
    url: 'https://youtu.be/dQw4w9WgXcQ',
    quality: '720p',
    apitoken: 'SUA_KEY'
  }
});

console.log(data);
```

</details>

<details>
<summary>📦 <strong>cURL (Terminal)</strong></summary>

```bash
curl -G "https://waguapis.online/download" \
  --data-urlencode "url=https://youtu.be/dQw4w9WgXcQ" \
  -d "quality=720p&apitoken=SUA_KEY"
```

</details>

<details>
<summary>📦 <strong>Request (Node.js)</strong></summary>

```javascript
request.get({
  url: 'https://waguapis.online/download',
  qs: {
    url: 'https://youtu.be/dQw4w9WgXcQ',
    quality: '720p',
    apitoken: 'SUA_KEY'
  },
  json: true
}, (err, res, body) => console.log(body));
```

</details>

**Retorno JSON (`200 OK`):**

```json
{
  "status": true,
  "title": "Never Gonna Give You Up",
  "quality": "720p",
  "size": "24.5 MB",
  "duration": "3:32",
  "download_url": "https://waguapis.online/cdn/downloads/xyz987.mp4",
  "thumbnail": "https://i.ytimg.com/vi/dQw4w9WgXcQ/hq720.jpg"
}
```

---

## 🛠️ Ferramentas de integração

A API WAGURI é compatível com qualquer cliente HTTP. Abaixo os mais utilizados:

| Ferramenta | Ambiente | Instalação |
|------------|----------|------------|
| **Fetch** | JavaScript (Browser / Node 18+) | Nativo |
| **Axios** | Node.js | `npm install axios` |
| **cURL** | Terminal / Shell | Nativo no Linux/macOS |
| **Request** | Node.js (legado) | `npm install request` |
| **Got** | Node.js moderno | `npm install got` |
| **Requests** | Python | `pip install requests` |

**Exemplo Python (Requests):**

```python
import requests

res = requests.get('https://waguapis.online/yt-search', params={
    'titulo': 'matuê 1993',
    'apitoken': 'SUA_KEY'
})

print(res.json())
```

---

## ❌ Erros comuns

| Código | Nome | Causa | Solução |
|--------|------|-------|---------|
| `400` | Bad Request | Parâmetro obrigatório ausente ou inválido | Verifique os parâmetros da rota |
| `401` | Unauthorized | Token inválido ou ausente | Confira o `apitoken` |
| `404` | Not Found | Rota inexistente | Verifique o endpoint |
| `429` | Rate Limit | Limite de requisições atingido | Aguarde ou faça upgrade do plano |
| `500` | Internal Error | Erro interno do servidor | Tente novamente ou contate o suporte |

**Exemplo de erro `401`:**

```json
{
  "status": false,
  "error": "Unauthorized",
  "message": "Token inválido ou não informado.",
  "code": 401
}
```

---

## 👨‍💻 Criador

<div align="center">

<img src="https://raw.githubusercontent.com/zenomdevs/uploads/main/016yf3.jpeg" width="100" style="border-radius:50%;" />

### uzuback

*Transformando ideias em sistemas inteligentes, APIs modernas e experiências visuais únicas.*

[![Instagram](https://img.shields.io/badge/Instagram-%40uzuback-ec4899?style=for-the-badge&logo=instagram&labelColor=0d1117)](https://instagram.com/uzuback)
[![Plataforma](https://img.shields.io/badge/Plataforma-waguapis.online-8b5cf6?style=for-the-badge&labelColor=0d1117)](https://waguapis.online)

</div>

---

## 📄 Licença

```
© 2026 WAGURI API's — Todos os direitos reservados.
Desenvolvido por uzuback. Uso não autorizado é proibido.
Para adquirir acesso, entre em contato via Instagram: @uzuback
```

---

<div align="center">

**Feito com 🟣 por [uzuback](https://instagram.com/uzuback)**

<a href="https://waguapis.online">
  <img src="https://img.shields.io/badge/%F0%9F%9A%80%20Acessar%20Plataforma-waguapis.online-8b5cf6?style=for-the-badge&labelColor=1a0a2e&color=8b5cf6" />
</a>

</div>
