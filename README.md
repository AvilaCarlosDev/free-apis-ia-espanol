# 🆓 Free APIs IA en Español

**Lista curada de APIs gratuitas de Inteligencia Artificial con documentación y ejemplos en español.**

---

## 📋 Descripción

Repositorio dedicado a recopilar APIs de IA que sean:
- ✅ **Gratuitas** - Sin costo o con tier free generoso
- ✅ **Documentadas en español** - O fácilmente traducibles
- ✅ **Funcionales** - Probadas y verificadas
- ✅ **Útiles** - Casos de uso prácticos

---

## 🎯 Objetivo

Ayudar a desarrolladores hispanohablantes a acceder a herramientas de IA sin barreras de idioma ni costos iniciales.

---

## 📚 Categorías

### 🗣️ Procesamiento de Lenguaje Natural (NLP)

| API | Descripción | Free Tier | Docs ES |
|-----|-------------|-----------|---------|
| **Hugging Face Inference** | Modelos pre-entrenados | 30k/mes gratis | ❌ |
| **LanguageTool** | Corrector gramatical | 20k/día | ✅ |
| **LibreTranslate** | Traducción open-source | Self-hosted | ✅ |

### 🖼️ Visión por Computadora

| API | Descripción | Free Tier | Docs ES |
|-----|-------------|-----------|---------|
| **ClearML** | MLOps y visión | Tier free | ❌ |
| **Roboflow** | Detección de objetos | 10k imágenes/mes | ❌ |

### 🤖 Chatbots y Asistentes

| API | Descripción | Free Tier | Docs ES |
|-----|-------------|-----------|---------|
| **Ollama** | Modelos locales | 100% gratis | ✅ (comunidad) |
| **LM Studio** | LLMs locales | 100% gratis | ❌ |

### 🎨 Generación de Imágenes

| API | Descripción | Free Tier | Docs ES |
|-----|-------------|-----------|---------|
| **Stable Diffusion Online** | Generación de imágenes | Limitado | ❌ |
| **Craiyon** | DALL-E mini | Gratis con ads | ❌ |

### 🔊 Audio y Voz

| API | Descripción | Free Tier | Docs ES |
|-----|-------------|-----------|---------|
| **Whisper (OpenAI)** | Transcripción | 100% gratis (local) | ✅ (comunidad) |
| **Coqui TTS** | Texto a voz | 100% gratis | ❌ |

---

## 🚀 Ejemplos de Uso

### Ollama - Modelo Local

```bash
# Instalar Ollama
curl -fsSL https://ollama.ai/install.sh | sh

# Descargar modelo en español
ollama pull llama2-es

# Ejecutar
ollama run llama2-es "Hola, ¿cómo estás?"
```

### Hugging Face - Inference API

```python
from huggingface_hub import InferenceClient

client = InferenceClient(token="hf_xxx")

response = client.text_generation(
    "El futuro de la IA es",
    model="mistralai/Mistral-7B-Instruct-v0.1"
)

print(response)
```

### LibreTranslate - Traducción

```bash
# Docker
docker run -ti --rm -p 5000:5000 libretranslate/libretranslate

# API call
curl -X POST "http://localhost:5000/translate" \
  -H "Content-Type: application/json" \
  -d '{
    "q": "Hello world",
    "source": "en",
    "target": "es"
  }'
```

---

## 📊 Criterios de Inclusión

Para que una API sea incluida en esta lista debe:

1. **Tener tier free** - Al menos 1000 requests/mes gratis
2. **Ser funcional** - Probada personalmente
3. **Tener documentación** - Aunque sea en inglés
4. **Ser útil** - Casos de uso reales

---

## 🛠️ Cómo Contribuir

1. Fork del repositorio
2. Agrega la API en la categoría correspondiente
3. Incluye:
   - Nombre y descripción
   - Link a la API
   - Detalles del free tier
   - Ejemplo de uso
4. Envía un PR

---

## 📝 Recursos Adicionales

- [Hugging Face Courses en Español](https://huggingface.co/learn)
- [Ollama Models](https://ollama.ai/library)
- [Awesome AI APIs](https://github.com/awesome-ai/awesome-ai-apis)

---

## ⚠️ Disclaimer

- Los free tiers pueden cambiar sin previo aviso
- Verifica siempre los términos de uso
- Para producción, considera planes pagos

---

## 📄 License

MIT License

---

*Workspace mantenido por Carlos Avila - Developer 🇻🇪*
