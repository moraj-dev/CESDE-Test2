# CESDE-Test2
PROGRAMA TÉCNICO LABORAL COMO ASISTENTE EN DESARROLLO DE  SOFTWARE

# 📌 Proyecto de Administración de Cursos y Docentes con JSON-Server

Este proyecto permite administrar **docentes y cursos** usando `json-server` como backend y una interfaz frontend en **HTML + Bootstrap + JavaScript**.

## 🚀 Características
✅ CRUD completo para **docentes** y **cursos**  
✅ API REST simulada con `json-server`  
✅ Uso de `fetch` para consumir la API  
✅ Diseño moderno y responsive con Bootstrap  
✅ Filtros y relaciones entre cursos y docentes  

---

## 📌 1️⃣ Instalación y Ejecución

### 🔹 **1. Clonar el repositorio**
```sh
git clone https://github.com/tuusuario/mi-proyecto.git
cd mi-proyecto

#Instalar json-server (Si no lo tienes)
npm install -g json-server
🔹 3. Iniciar el servidor JSON

#Levantar el servidor en un puerto especifico. En el ejemplo sera el puerto por defecto: 3000
json-server --watch db.json --port 3000

# Uso del Proyecto
#🔹 Abrir la interfaz en el navegador
#Página principal: index.html
#Administrar Docentes: docentes.html
#Administrar Cursos: cursos.html
#📌 3️⃣ Endpoints de la API
#📚 Cursos
#Método	Endpoint	Descripción
#GET	/cursos	Obtener todos los cursos
#GET	/cursos?id=1	Obtener un curso por ID
#POST	/cursos	Crear un curso
#PUT	/cursos?id=1	Actualizar un curso
#DELETE	/cursos?id=1	Eliminar un curso
#👨‍🏫 Docentes
#Método	Endpoint	Descripción
#GET	/docentes	Obtener todos los docentes
#GET	/docentes?docente_id=1	Obtener un docente por ID
#POST	/docentes	Crear un docente
#PUT	/docentes?docente_id=1	Actualizar un docente
#DELETE	/docentes?docente_id=1	Eliminar un docente
#📌 4️⃣ Relación Cursos - Docentes
#Cada curso tiene un docente_id que referencia a un docente.
#Para obtener un curso con la información del docente:
GET http://localhost:3000/cursos?_expand=docente
GET http://localhost:3000/docentes/1?_embed=cursos

#5️⃣ Tecnologías Usadas
#JSON-Server 🗄️ (API REST falsa)
#HTML, CSS y JavaScript 🎨

#IMPORTANTE
#En el proyecto se encuentra la base de datos en archivo JSON (db.json)


