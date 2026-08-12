# 🌐 Soluciones Integrales JB

<p align="center">
  <strong>Plataforma web corporativa Full Stack con integración de Inteligencia Artificial</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-5.8-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Vite-7-646CFF?style=for-the-badge&logo=vite&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-Backend-339933?style=for-the-badge&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-5-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/Ollama-AI-black?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Vercel-Deployment-000000?style=for-the-badge&logo=vercel&logoColor=white" />
</p>

---

## 📌 Descripción

**Soluciones Integrales JB** es una plataforma web corporativa desarrollada para presentar los servicios, información institucional y soluciones tecnológicas de la empresa.

El proyecto fue desarrollado como una aplicación **Full Stack**, combinando un frontend moderno construido con **React + TypeScript + Vite**, un backend basado en **Node.js + Express**, integración con **MySQL** y funcionalidades de **Inteligencia Artificial mediante Ollama**.

La aplicación está diseñada para ofrecer una experiencia moderna, responsive e interactiva, incorporando navegación por rutas, componentes reutilizables, animaciones, carruseles, integración de servicios y un asistente virtual.

---

## 🚀 Características principales

### 🌐 Plataforma corporativa

* Presentación de la empresa y su propuesta de valor.
* Secciones institucionales.
* Información del equipo.
* Presentación de servicios.
* Sección de contacto.
* Navegación mediante rutas.
* Diseño responsive para diferentes dispositivos.

### 🧩 Interfaz y experiencia de usuario

* Componentes reutilizables.
* Animaciones e interacciones.
* Carruseles.
* Galerías visuales.
* Botones de navegación.
* Navegación fluida entre páginas.
* Elementos visuales interactivos.
* Diseño orientado a una experiencia moderna.

### 🏢 Servicios representados

La plataforma incluye diferentes áreas de servicio, entre ellas:

* Desarrollo de sitios web.
* Desarrollo de software.
* Soporte técnico.
* Redes e infraestructura.
* Seguridad informática.
* Tecnología en seguridad.
* Consultoría TI.
* Consultoría empresarial.
* Consultoría educativa.
* Facturación electrónica.
* Hosting y dominios.
* Posicionamiento SEO.
* Social Media.
* Gráfica publicitaria.
* Merchandising.
* Instalaciones eléctricas.
* Refrigeración industrial.

---

# 🤖 Integración de Inteligencia Artificial

Uno de los componentes principales del proyecto es la integración de un **asistente virtual basado en Inteligencia Artificial**.

La solución utiliza **Ollama** para ejecutar un modelo local y generar respuestas contextualizadas para los visitantes.

El asistente está configurado para comprender consultas relacionadas con los servicios de la empresa y orientar al usuario hacia la solución correspondiente.

### 🧠 Funcionamiento

El flujo general es:

```text
Usuario
   │
   ▼
Asistente Web
   │
   ▼
API /api/chat
   │
   ├── Respuestas rápidas
   │
   ├── Respuestas locales
   │
   └── Ollama
          │
          ▼
      Modelo de IA
          │
          ▼
      Respuesta
```

La API mantiene parte del contexto de conversación y limita la cantidad de mensajes enviados al modelo para controlar el procesamiento.

También existe un sistema de **fallback**, permitiendo entregar respuestas locales cuando el proveedor de IA no está disponible.

---

# 🏗️ Arquitectura

El proyecto utiliza una arquitectura dividida en diferentes capas:

```text
                    ┌──────────────────────┐
                    │       Usuario        │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │      Frontend        │
                    │ React + TypeScript   │
                    │        + Vite        │
                    └──────────┬───────────┘
                               │
                ┌──────────────┴──────────────┐
                │                             │
                ▼                             ▼
       ┌─────────────────┐          ┌─────────────────┐
       │ Backend Express │          │ Serverless API  │
       │   Node.js       │          │    Vercel       │
       └────────┬────────┘          └────────┬────────┘
                │                            │
                ▼                            ▼
       ┌─────────────────┐          ┌─────────────────┐
       │      MySQL      │          │     Ollama      │
       │    Database     │          │   AI / LLM      │
       └─────────────────┘          └─────────────────┘
```

---

# 🛠️ Stack Tecnológico

## Frontend

* React 19
* TypeScript
* Vite
* React Router
* Bootstrap
* Tailwind CSS
* Framer Motion
* GSAP
* Three.js
* React Three Fiber
* React Icons
* Lucide React
* Swiper
* React Slick

Las dependencias principales del frontend están definidas en `package.json`.

## Backend

* Node.js
* Express 5
* CORS
* dotenv
* Axios
* MySQL2

El backend dispone de endpoints para funcionalidades de la plataforma y conexión con MySQL.

## Base de datos

* MySQL
* MySQL2

La aplicación utiliza variables de entorno para configurar la conexión a la base de datos.

## Inteligencia Artificial

* Ollama
* Modelos LLM locales
* API de Ollama
* Contexto conversacional
* Respuestas locales de respaldo

## Deployment

* Vercel
* Serverless Functions
* Vercel Rewrites

El proyecto incluye configuración específica para enrutar las solicitudes `/api/*` mediante Vercel.

---

# 📂 Estructura del proyecto

```text
PROYECTO-SOLUCIONES-INTEGRALES/
│
├── api/
│   └── chat.js
│
├── backend/
│   ├── index.js
│   ├── package.json
│   └── .env
│
├── public/
│
├── src/
│   ├── assets/
│   ├── backups/
│   │
│   ├── components/
│   │   ├── CircularGallery.tsx
│   │   ├── LogoLoop.tsx
│   │   ├── Productos.tsx
│   │   ├── ScrollButton.tsx
│   │   ├── SolucionesIntegralesJBSection.tsx
│   │   ├── TestimoniosCarousel.tsx
│   │   ├── VoiceflowChat.jsx
│   │   ├── navbar.tsx
│   │   └── footer.tsx
│   │
│   ├── lib/
│   │
│   ├── pages/
│   │   ├── QuienesSomos.tsx
│   │   ├── NuestroEquipo.tsx
│   │   ├── DesarrolloDeSitiosWeb.tsx
│   │   ├── DesarrolloDeSoftware.tsx
│   │   ├── FacturacionElectronica.tsx
│   │   ├── SoporteTecnico.tsx
│   │   ├── RedesEInfrostructura.tsx
│   │   ├── SeguridadInfromatica.tsx
│   │   ├── ConsultoriaTI.tsx
│   │   ├── Contacto.tsx
│   │   └── ...
│   │
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css
│
├── package.json
├── vite.config.ts
├── tailwind.config.js
├── vercel.json
└── README.md
```

La estructura actual contiene una separación clara entre componentes reutilizables, páginas, API y backend.

---

# ⚙️ Instalación

## 1. Clonar el repositorio

```bash
git clone https://github.com/jaredaalarcon-dev/PROYECTO-SOLUCIONES-INTEGRALES.git
```

```bash
cd PROYECTO-SOLUCIONES-INTEGRALES
```

---

## 2. Instalar dependencias del frontend

```bash
npm install
```

---

## 3. Ejecutar el frontend

```bash
npm run dev
```

La aplicación se ejecutará mediante el servidor de desarrollo de Vite.

---

# ⚙️ Configuración del Backend

Ingresar a:

```bash
cd backend
```

Instalar dependencias:

```bash
npm install
```

Ejecutar:

```bash
npm start
```

El backend está configurado para ejecutarse mediante Node.js y Express.

---

# 🔐 Variables de entorno

Las credenciales y configuraciones sensibles deben mantenerse fuera del repositorio.

Ejemplo:

```env
PORT=3006

DB_HOST=localhost
DB_USER=usuario
DB_PASSWORD=contraseña
DB_NAME=base_de_datos

OLLAMA_BASE_URL=http://127.0.0.1:11434
OLLAMA_MODEL=llama3.2:1b
OLLAMA_TIMEOUT_MS=6000
```

> ⚠️ **Importante:** nunca publiques contraseñas, tokens, API keys o credenciales reales en GitHub.

---

# 🤖 Configuración de Ollama

Instala Ollama en el entorno donde se ejecutará el backend y asegúrate de tener disponible el modelo configurado.

Por defecto, el proyecto contempla:

```env
OLLAMA_BASE_URL=http://127.0.0.1:11434
OLLAMA_MODEL=llama3.2:1b
```

El backend utiliza el endpoint `/api/chat` de Ollama para generar las respuestas del asistente virtual.

---

# 🧪 Scripts disponibles

## Frontend

```bash
npm run dev
```

Inicia el servidor de desarrollo.

```bash
npm run build
```

Genera la versión de producción.

```bash
npm run lint
```

Ejecuta ESLint.

```bash
npm run preview
```

Previsualiza el build de producción.

Estos scripts están definidos actualmente en `package.json`.

## Backend

```bash
npm start
```

Inicia el servidor Express.

```bash
npm run dev
```

Ejecuta el backend en modo desarrollo.

---

# 📡 API

### POST `/api/chat`

Endpoint utilizado por el asistente virtual.

Ejemplo de solicitud:

```json
{
  "messages": [
    {
      "from": "user",
      "text": "Necesito una página web"
    }
  ]
}
```

La API procesa la conversación y puede responder mediante:

* Respuestas conocidas.
* Respuestas rápidas.
* Respuestas locales.
* Modelo de Inteligencia Artificial mediante Ollama.

---

### GET `/productos`

Endpoint del backend utilizado para consultar productos almacenados en MySQL.

```http
GET /productos
```

La implementación actual consulta la tabla `products`.

---

# 📱 Diseño Responsive

La interfaz está desarrollada para adaptarse a diferentes tamaños de pantalla, utilizando componentes y estilos orientados a dispositivos móviles, tablets y desktop.

---

# 🎨 Componentes destacados

Entre los componentes desarrollados se encuentran:

* Navbar
* Footer
* Carruseles
* Galerías
* Botones de navegación
* Animaciones
* Testimonios
* Productos
* Secciones corporativas
* Asistente virtual
* Elementos interactivos

La carpeta `src/components` contiene actualmente componentes específicos para estas funcionalidades.

---

# 📈 Estado del proyecto

**Estado:** 🟢 Activo / En desarrollo

El proyecto continúa evolucionando con nuevas funcionalidades, mejoras visuales, optimización de componentes e integración de nuevas soluciones tecnológicas.

---

# 🔮 Próximas mejoras

Algunas mejoras que pueden incorporarse:

* [ ] Optimización del rendimiento.
* [ ] Mejoras adicionales de accesibilidad.
* [ ] Pruebas automatizadas.
* [ ] Documentación técnica ampliada.
* [ ] Mejoras en observabilidad y manejo de errores.
* [ ] Mayor cobertura de endpoints.
* [ ] Mejoras en la integración de IA.
* [ ] Optimización de la experiencia móvil.

---

# 👨‍💻 Autor

### Jared Alonso Arroyo Alarcon

**Software Engineer | Full Stack Developer | AI**

🔗 GitHub:
https://github.com/jaredaalarcon-dev

🔗 LinkedIn:
https://www.linkedin.com/in/jared-alonso-arroyo-alarcon-b95993399/

🔗 Pagina Web:
https://solucionesintegralesjb.com/

---

<p align="center">
  <strong>Construyendo soluciones de software modernas con tecnología e Inteligencia Artificial.</strong>
</p>
```

### Una mejora importante que hice respecto al README anterior

No inventé tecnologías ni funcionalidades que no aparecen en el proyecto. Por ejemplo, el `package.json` confirma React 19, TypeScript 5.8, Vite 7, React Router, Three.js, GSAP, Framer Motion, etc.

Y el backend confirma **Express, MySQL2, CORS, dotenv y Axios**, mientras que el código confirma la integración directa con Ollama y el endpoint `/api/chat`.

### 🚨 Pero antes de hacer commit

**No quiero que simplemente pegues esto y ya.** Hay una cosa que debemos solucionar primero:

> `backend/.env`

El repositorio público muestra ese archivo en el árbol del backend.

Si ese `.env` contiene **credenciales reales de MySQL, tokens o cualquier secreto**, hay que sacarlo del repositorio y, si alguna credencial real llegó a estar publicada, **cambiarla/rotarla**.

Después de eso sí hacemos el commit del README.

Y una vez que terminemos con la seguridad, el siguiente paso que te recomiendo es **poner capturas reales de tu aplicación dentro del README**. Eso hará que este repositorio pase de verse como documentación técnica a verse como un **proyecto de portfolio profesional**.
