# Desafio-like-me-parte1-Mariel-Montoya
# Desafío Like Me — Parte I

Aplicación Full Stack desarrollada como desafío académico que permite crear publicaciones con imagen, descripción y sistema de likes utilizando React en el frontend y Node.js + Express + PostgreSQL en el backend.

---

## Tecnologías utilizadas

### Frontend
- React
- Vite
- CSS

### Backend
- Node.js
- Express
- PostgreSQL
- pg (node-postgres)
- cors

### Control de versiones
- Git
- GitHub

---

## Instalación y ejecución

### Backend

```bash
cd server
npm install
npm run dev
Servidor disponible en:

http://localhost:3000

Frontend
bash
Copiar código
cd client
npm install
npm run dev
Aplicación disponible en:

http://localhost:5173

Configuración de Base de Datos
Crear base PostgreSQL llamada:

nginx
Copiar código
likeme
Crear tabla requerida
sql
Copiar código
CREATE TABLE posts (
    id SERIAL PRIMARY KEY,
    titulo VARCHAR(255),
    img VARCHAR(1000),
    descripcion VARCHAR(255),
    likes INTEGER DEFAULT 0
);
Endpoints principales
Método	Ruta	Descripción
GET	/posts	Obtener publicaciones
POST	/posts	Crear publicación
PUT	/posts/like/:id	Incrementar likes
DELETE	/posts/:id	Eliminar publicación

Estructura del proyecto
pgsql
Copiar código
client/
server/
client → Aplicación React

server → API Node/Express + PostgreSQL

Autora
Mariel A. Montoya
