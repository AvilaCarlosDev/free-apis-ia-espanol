# 🆓 Free LLM APIs en Español

**Lista curada de recursos gratuitos de LLM e IA accesibles vía API - Para la comunidad hispanohablante.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Stars](https://img.shields.io/github/stars/AvilaCarlosDev/free-apis-ia-espanol)](https://github.com/AvilaCarlosDev/free-apis-ia-espanol/stargazers)

---

## ⚠️ Aviso Importante

> **Por favor, no abuses de estos servicios gratuitos.** Si abusamos, podríamos perderlos.
> 
> Esta lista excluye explícitamente servicios que no son legítimos (ej: que hacen ingeniería inversa de chatbots existentes).

---

## 📚 Tabla de Contenidos

- [Proveedores 100% Gratuitos](#-proveedores-100-gratuitos)
- [Proveedores con Créditos de Prueba](#-proveedores-con-créditos-de-prueba)
- [Modelos Locales (Sin Límites)](#-modelos-locales-sin-límites)
- [Comparativa de Límites](#-comparativa-de-límites)
- [Ejemplos de Código](#-ejemplos-de-código)
- [Cómo Contribuir](#-cómo-contribuir)

---

## 🆓 Proveedores 100% Gratuitos

### [OpenRouter](https://openrouter.ai) 🔥

**Límites:**
- 20 requests/minuto
- 50 requests/día
- Hasta 1000 requests/día con $10 de top-up lifetime

**Modelos Gratuitos Disponibles:**

| Modelo | Provider | Contexto |
|--------|----------|----------|
| Gemma 3 27B Instruct | Google | 8K |
| Gemma 3 12B Instruct | Google | 8K |
| Llama 3.3 70B Instruct | Meta | 8K |
| Llama 3.2 3B Instruct | Meta | 8K |
| Qwen 2.5 Coder 32B | Alibaba | 8K |
| Mistral 7B Instruct | Mistral AI | 8K |
| DeepSeek R1 | DeepSeek | 8K |

**Ejemplo de uso:**
```bash
curl https://openrouter.ai/api/v1/chat/completions \
  -H "Authorization: Bearer $OPENROUTER_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "meta-llama/llama-3.3-70b-instruct:free",
    "messages": [{"role": "user", "content": "Hola, ¿cómo estás?"}]
  }'
```

---

### [Google AI Studio](https://aistudio.google.com) 🇬

**Requiere:** Cuenta de Google

**Límites por modelo:**

| Modelo | Tokens/minuto | Requests/día |
|--------|---------------|--------------|
| Gemini 2.5 Flash | 250,000 | 20 |
| Gemini 2.5 Flash-Lite | 250,000 | 20 |
| Gemma 3 27B Instruct | 15,000 | 14,400 |
| Gemma 3 12B Instruct | 15,000 | 14,400 |
| Gemma 3 4B Instruct | 15,000 | 14,400 |

**Nota:** Los datos se usan para training fuera de UK/CH/EEA/EU.

---

### [NVIDIA NIM](https://build.nvidia.com/explore/discover) 🟢

**Requiere:** Verificación con número de teléfono

**Límites:**
- 40 requests/minuto
- Modelos limitados por contexto

**Modelos disponibles:** Varios modelos open-source de NVIDIA

---

### [Mistral La Plateforme](https://console.mistral.ai/) 🔵

**Plan:** Experiment (Free)

**Requiere:** Verificación con teléfono

**Límites (por modelo):**
- 1 request/segundo
- 500,000 tokens/minuto
- 1,000,000,000 tokens/mes

**Modelos:** Mistral Open y Proprietary

---

### [HuggingFace Inference](https://huggingface.co/docs/inference-providers/) 🤗

**Límites:** ~$0.10/mes en créditos gratuitos

**Proveedores soportados:**
- HF Serverless Inference
- Replicate
- Fal.ai
- Novita

**Modelos:** Varios modelos open-source < 10GB

---

### [Groq](https://console.groq.com) ⚡

**Velocidad:** Inferencia ultra-rápida

**Límites por modelo:**

| Modelo | Requests/día | Tokens/minuto |
|--------|--------------|---------------|
| Llama 3.1 8B | 14,400 | 6,000 |
| Llama 3.3 70B | 1,000 | 12,000 |
| Llama 4 Scout | 1,000 | 30,000 |
| Whisper Large v3 | 7,200 audio-seg/min | 2,000 |

---

### [Cohere](https://cohere.com) 🔷

**Límites:**
- 20 requests/minuto
- 1,000 requests/mes

**Modelos:**
- Command R+ (08-2024)
- Command R (08-2024)
- Command A (03-2025)
- Aya Expanse 32B

---

### [GitHub Models](https://github.com/marketplace/models) 💻

**Límites:** Dependen del tier de Copilot

| Tier | Límite |
|------|--------|
| Free | 200 requests/mes |
| Pro | 2,000 requests/mes |
| Pro+ | 8,000 requests/mes |
| Business | 80,000 requests/mes |

**Modelos destacados:**
- GPT-4o, GPT-4o mini
- Llama 3.1/3.2/3.3
- Mistral Small/Medium
- DeepSeek R1/V3
- Phi-4

---

### [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai) ☁️

**Límites:** 10,000 neurons/día (~$0.50 valor)

**Modelos populares:**
- @cf/meta/llama-3.2-11b-vision-instruct
- @cf/meta/llama-3.2-3b-instruct
- @cf/google/gemma-4-26b-a4b-it
- @cf/qwen/qwen3-30b-a3b-fp8
- DeepSeek R1 Distill Qwen 32B

---

## 💰 Proveedores con Créditos de Prueba

### [Fireworks](https://fireworks.ai/)
- **Créditos:** $1 USD
- **Modelos:** Varios open models

### [Baseten](https://app.baseten.co/)
- **Créditos:** $30 USD
- **Modelos:** Cualquier modelo soportado (pago por tiempo de cómputo)

### [Nebius](https://tokenfactory.nebius.com/)
- **Créditos:** $1 USD
- **Modelos:** Varios open models

### [Novita](https://novita.ai/)
- **Créditos:** $0.50 USD (1 año)
- **Modelos:** Varios open models

### [AI21](https://studio.ai21.com/)
- **Créditos:** $10 USD (3 meses)
- **Modelos:** Familia Jamba

### [Upstage](https://console.upstage.ai/)
- **Créditos:** $10 USD (3 meses)
- **Modelos:** Solar Pro/Mini

### [Alibaba Cloud Model Studio](https://bailian.console.alibabacloud.com/)
- **Créditos:** 1 millón de tokens/modelo
- **Modelos:** Qwen (varios)

---

## 🖥️ Modelos Locales (Sin Límites)

### [Ollama](https://ollama.ai)

**Costo:** 100% gratis (corre local)

**Instalación:**
```bash
curl -fsSL https://ollama.ai/install.sh | sh
```

**Modelos en español recomendados:**
```bash
ollama pull llama2-es
ollama pull gemma:7b-es
ollama pull mistral:7b-instruct-v0.2-q4_K_M
```

**Límites:** Dependen de tu hardware (RAM, GPU)

---

### [LM Studio](https://lmstudio.ai/)

**Costo:** 100% gratis (interfaz gráfica)

**Features:**
- Interfaz visual amigable
- Descarga modelos desde HuggingFace
- API local compatible con OpenAI

---

### [LocalAI](https://localai.io/)

**Costo:** 100% gratis (self-hosted)

**Features:**
- API drop-in replacement de OpenAI
- Soporta múltiples backends
- Ideal para producción local

---

## 📊 Comparativa de Límites

| Provider | Free Tier | Requiere Phone | Data para Training |
|----------|-----------|----------------|-------------------|
| OpenRouter | ✅ 50/day | ❌ | ❌ (free tier) |
| Google AI Studio | ✅ 250K tokens/min | ❌ | ✅ (fuera de EU) |
| NVIDIA NIM | ✅ 40/min | ✅ | ❌ |
| Mistral | ✅ 1B tokens/mes | ✅ | ✅ (opt-in) |
| Groq | ✅ 14K/day | ❌ | ❌ |
| GitHub Models | ✅ 200/mes (Free) | ❌ | ❌ |
| Cloudflare | ✅ 10K neurons/day | ❌ | ❌ |
| Ollama (local) | ✅ Ilimitado | ❌ | ❌ |

---

## 💻 Ejemplos de Código

### Python - OpenRouter

```python
import requests

response = requests.post(
    "https://openrouter.ai/api/v1/chat/completions",
    headers={
        "Authorization": f"Bearer {os.getenv('OPENROUTER_KEY')}"
    },
    json={
        "model": "meta-llama/llama-3.3-70b-instruct:free",
        "messages": [
            {"role": "user", "content": "Hola, ¿cómo estás?"}
        ]
    }
)

print(response.json()['choices'][0]['message']['content'])
```

### JavaScript/Node - Groq

```javascript
import Groq from 'groq-sdk';

const groq = new Groq({ apiKey: process.env.GROQ_API_KEY });

const response = await groq.chat.completions.create({
  model: 'llama-3.3-70b-versatile',
  messages: [{ role: 'user', content: 'Hola, ¿cómo estás?' }]
});

console.log(response.choices[0].message.content);
```

### Bash - Ollama Local

```bash
#!/bin/bash
# script-ollama.sh

curl http://localhost:11434/api/generate -d '{
  "model": "llama2-es",
  "prompt": "Explica qué es una API",
  "stream": false
}'
```

---

## 🛠️ Cómo Contribuir

### Agregar un Nuevo Provider

1. **Fork** este repositorio
2. **Crea una rama:** `git checkout -b feature/add-provider-x`
3. **Agrega la sección** siguiendo el formato existente
4. **Incluye:**
   - Nombre y link oficial
   - Límites exactos (requests, tokens, etc.)
   - Modelos disponibles
   - ¿Requiere verificación?
   - ¿Usa datos para training?
5. **Envía un PR** con descripción clara

### Formato de Contribución

```markdown
### [Nombre del Provider](https://url.com)

**Límites:**
- X requests/minuto
- Y requests/día

**Requiere:** [Teléfono/Tarjeta/None]

**Modelos:** Lista de modelos disponibles
```

---

## 📝 Recursos Adicionales

### En Español
- [Hugging Face Courses ES](https://huggingface.co/learn)
- [Ollama Models](https://ollama.ai/library)
- [Curso de IA - 4Geeks Academy](https://4geeksacademy.co/)

### En Inglés
- [Awesome AI APIs](https://github.com/awesome-ai/awesome-ai-apis)
- [There's An AI For That](https://theresanaiforthat.com/)
- [AI Models Directory](https://ai-models.info/)

---

## ⚠️ Disclaimer

- Los free tiers pueden cambiar sin previo aviso
- Verifica siempre los términos de uso actuales
- Para producción, considera planes pagos para estabilidad
- No uses estos servicios para spam o abuse

---

## 📄 Licencia

MIT License - ver [LICENSE](./LICENSE) para detalles.

---

## 🌟 Agradecimientos

- Inspirado en [free-llm-api-resources](https://github.com/cheahjs/free-llm-api-resources)
- Traducido y adaptado para la comunidad hispanohablante
- Mantenido por [@AvilaCarlosDev](https://github.com/AvilaCarlosDev)

---

*Workspace mantenido por Carlos Avila - Developer 🇻🇪*
