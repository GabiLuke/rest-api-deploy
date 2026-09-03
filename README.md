# 🎬 REST API de Películas — Node + Express

API REST de películas construida con **Express**, con validación de datos mediante **Zod**, filtrado por género y configuración de **CORS** por origen. Incluye un cliente web mínimo para consumirla.

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)
![Zod](https://img.shields.io/badge/Zod-3E67B1?style=flat&logo=zod&logoColor=white)

---

## ✨ Funcionalidades

- 📋 CRUD completo de películas (`GET`, `POST`, `PATCH`, `DELETE`)
- 🔎 Filtrado por género (`/movies?genre=Action`)
- ✅ **Validación de datos** de entrada con esquemas Zod
- 🌐 **CORS** con lista de orígenes permitidos
- 🧾 Cabecera `x-powered-by` deshabilitada (buena práctica de seguridad)

---

## 🛠️ Stack técnico

| Tema | Detalle |
|------|---------|
| Runtime | Node.js · Express 5 |
| Validación | Zod |
| Otros | CORS · `crypto.randomUUID()` |

---

## 📡 Endpoints

| Método | Ruta | Descripción |
|--------|------|-------------|
| `GET` | `/movies` | Lista todas las películas (o filtra por `?genre=`) |
| `GET` | `/movies/:id` | Devuelve una película por su id |
| `POST` | `/movies` | Crea una película (valida el body) |
| `PATCH` | `/movies/:id` | Actualiza parcialmente una película |
| `DELETE` | `/movies/:id` | Elimina una película |

> Puedes probar los endpoints con el archivo [`api.http`](api.http) incluido.

---

## 🚀 Puesta en marcha local

```bash
git clone https://github.com/GabiLuke/rest-api-deploy.git
cd rest-api-deploy
npm install
npm start     # http://localhost:1234
```

---

## 🎯 Qué demuestra este proyecto

- Diseño de una **API REST** siguiendo las convenciones de métodos y códigos de estado HTTP.
- **Validación de entrada** desacoplada en esquemas reutilizables.
- Configuración de **CORS** por origen y nociones básicas de seguridad en cabeceras.

> Los datos se almacenan en memoria (`movies.json`), por lo que los cambios no persisten al reiniciar. Es un proyecto de aprendizaje centrado en el diseño de la API y su despliegue.

---

## 👤 Autor

**Gabriel Luque Velasco** — Desarrollador Full-Stack Junior
[GitHub](https://github.com/GabiLuke) · [LinkedIn](#) · gabiluke99@gmail.com
