# 🤖 Agente Total – Asistente de IA Multicanal con Memoria y Herramientas

**Agente Total** es un agente de inteligencia artificial conversacional conectado a Telegram, diseñado para actuar como un asistente personal de alto rendimiento. Este agente combina interpretación de mensajes (texto y voz) con ejecución de tareas mediante múltiples herramientas especializadas.

---

## 🎯 Objetivo
Automatizar la asistencia diaria de un usuario, integrando funciones de:
- Procesamiento de texto y voz
- Gestión de correos electrónicos
- Creación y consulta de eventos en calendario
- Búsquedas en la web y Wikipedia
- Publicaciones en redes sociales
- Conversación contextualizada con memoria

---

## 🛠️ Tecnologías y Herramientas
- **n8n** (como orquestador principal)
- **Telegram API** (input/output)
- **OpenAI API (GPT + Whisper)** – procesamiento de lenguaje y transcripción
- **Google Calendar API** – gestión de eventos
- **Gmail API** – gestión de correos
- **Wikipedia / HackerNews / SerpAPI** – búsqueda web
- **MCP Client Tools** – ejecución de tareas externas
- **LangChain Memory Buffer** – contexto de conversación

---

## ⚙️ Funcionalidades

### 🔹 Entrada vía Telegram
- Mensajes de **texto** y **voz**
- Procesamiento del input según el tipo y activación del flujo adecuado

### 🧠 Procesamiento con OpenAI
- GPT-4o como modelo principal para razonamiento
- Transcripción automática de audios con Whisper

### 📚 Memoria de contexto
- Implementación de ventana de memoria para mantener el historial de conversación en sesiones

### 🧰 Herramientas Inteligentes Integradas
| Herramienta         | Función                                                  |
|---------------------|----------------------------------------------------------|
| `Gmail_Tool`        | Leer, responder, redactar y etiquetar correos            |
| `Calendar_Tool`     | Crear, modificar, borrar y consultar eventos             |
| `search_agent`      | Búsqueda en Wikipedia, HackerNews, SerpAPI               |
| `x_posts`           | Redacción y publicación de contenido para redes sociales |

---

## 🧬 Arquitectura del flujo

![image](https://github.com/user-attachments/assets/86e0c240-c398-4175-b6b0-cc200f575bf6)
