# 🛠️ Proyecto Base: Node.js + Express + Sequelize
 
Este es un proyecto de inicio rápido (starter) para crear una aplicación backend con **Node.js**, **Express** y **Sequelize** conectada a una base de datos **PostgreSQL**.

> Ideal si estás empezando a construir tus propios proyectos o necesitas una plantilla para crear una API desde cero.

---

## ¿Qué incluye este proyecto?

-  **Express.js** para crear rutas y manejar solicitudes HTTP.
-  **Sequelize** como ORM para trabajar con bases de datos fácilmente.
-  **PostgreSQL** como base de datos relacional.
-  **dotenv** para manejar configuraciones privadas (como contraseñas).
-  **Nodemon** para reiniciar el servidor automáticamente en desarrollo.
-  Estructura limpia, lista para escalar.

---

## 📂 Estructura de Carpetas

Node.js-Express-Starter-01/

├── src/

│    ├── routes/   # Aquí van tus rutas (endpoints)

│    ├── utils/    # Herramientas útiles (manejadores de errores, conexión, etc.)

│    ├── app.js    # Configuración principal de la app

│    └── server.js # Punto de inicio del servidor

│

├── .env.example # Archivo de ejemplo para variables de entorno 

├── .gitignore   # Ignora archivos como node_modules y .env

├── package.json # Dependencias y scripts


---

## Cómo usar este proyecto como base para tus propios desarrollos

¿Quieres comenzar tu propio backend con esta misma estructura? Aquí te explico cómo hacerlo:

### Opción A: Usar como plantilla (recomendado si quieres empezar desde cero)

#### 1. Ve al repositorio original en GitHub (este repositorio xD)

#### 2. Haz click en el botón verde "Use this template/Create a new repository" (Usar esta plantilla/crear nuevo repositorio)

Esto te permitirá crear una copia nueva del repositorio en tu cuenta, sin el historial de cambios (commits) del original. Ideal para empezar limpio.

#### 3. Ponle un nuevo nombre a tu proyecto.

Por ejemplo: mi-api-rest, backend-tareas, o cualquier nombre que identifique tu aplicación.

#### 4. Clona tu nuevo repositorio a tu computadora:

Desde tu cuenta de GitHub en el repositorio copiado como template, copia el URL para clonarlo.

--- Depués de eso puedes pasar a la sección **Cómo comenzar** en este README

### Opción B: Fork (recomendado si quieres colaborar con este proyecto o mantenerlo sincronizado)

#### 1. Haz clic en el botón "Fork" en la esquina superior derecha del repositorio.

#### 2. Esto crea una copia de este proyecto en tu cuenta, con el historial de cambios completo.

Esta copia mantiene todo el historial de cambios (commits, ramas, issues si decides traerlos, etc.).

Pero esta copia sólo está en la nube, no en tu computadora aún. Necesitas clonarlo desde tu cuenta para trabajar en ese Fork.

#### 3. Clona el Fork a tu computadora. 

Desde tu cuenta de GitHub en el repositorio "Forkeado", copia el URL para clonarlo. 

---Después de eso puedes continuar en la sección **Cómo comenzar** (justo enseguida, abajo)


## Cómo comenzar

### 1. Clona el repositorio

#### Tanto si copiaste este repositorio como Template, como si lo hiciste con un Fork, el paso siguiente es clonarlo a tu entorno local. 

---En tu editor de Código (i.e. Visual Studio Code, o el que estés usando), ubícate en la carpeta en la que quieras clonar tu proyecto backend.

---Enseguida en tu terminal clonas el proyecto con ```git clone``` seguido de la URL que copiaste, ya sea del Fork o del Template

```git clone https://github.com/tu-usuario/Node-api-ejemplo-01.git```

---una vez clonado entra a la carpeta raíz del proyecto

```cd Node-api-ejemplo-01```

### 2. Instala las dependencias

  ```npm install```

  Esto creará la carpeta node-modules y un archivo package-lock.json

### 3. Configura tus variables de entorno

---Copia el contenido del archivo de ejemplo **.env.example** y pégalo en un nuevo archivo **.env** (puedes usar este comando):
 
  ```cp .env.example .env```

---Asegúrate de que tu base de datos esté creada y corriendo en PostgreSQL (-No necesitas hacer nada con la base de datos por ahora, solo crearla).

---Abre el archivo .env y reemplaza <nombre_db> por el nombre real de tu base de datos:

    ```DATABASE_URL=postgres://postgres:tu_contraseña@127.0.0.1:5432/nombre_real_de_tu_db```

### 4. Ejecuta el proyecto
---En desarrollo (con reinicios automáticos):

  ```npm run dev```

---En producción:

  ```npm start```
  
Esto quiere decir que mientras estés trabajando en tu computadora (modo desarrollo), 
puedes utilizar ```npm run dev```.
Este comando ejecuta el servidor usando Nodemon, que reinicia automáticamente tu aplicación cada vez que guardas un cambio en el código. Muy útil mientras estás programando.

Cuando quieras desplegar tu proyecto en la nube (por ejemplo en Render, Railway, AWS, GCP, Azure, Fl0, etc.), deberás asegurarte de que el comando configurado para iniciar la aplicación sea: ```npm start```.

Este comando ejecuta el servidor sin reinicios automáticos, como se espera en entornos de producción.

En plataformas como Render o Railway, normalmente puedes configurar el comando de inicio (start command), y ahí deberás escribir ```npm start```.

---Tras ejecutarlo verás algo como:

```DB connected```

```Server running on port 8080```


### ¿Y ahora qué?

A partir de aquí puedes:

* Crear una carpeta **models** en **src**, y crear tus modelos ahí.
* Agregar rutas nuevas dentro de ```src/routes/index.js```.
* Organizar tus controladores en una carpeta ```controllers``` dentro de **src**.
* Usar las herramientas incluídas (catchError.js, errorHandler.js) para mejorar el manejo de errores en tus controladores.


## ¿Por qué usar esta plantilla?

Porque te ahorra tiempo configurando lo básico y te permite enfocarte en desarrollar tu API sin preocuparte por la estructura inicial.
Ideal para prácticas, proyectos personales o incluso pruebas técnicas.

## ¿Tienes dudas?

No dudes en abrir un Issue en este repositorio, agregarme como colaborador a tu nuevo repositorio, 

O contactarme por correo ```beehiverm@gmail.com```.

Este README es solo para ayudarte a poner en marcha tu aplicación backend, pero si quieres llevar a término una API robusta con operaciones CRUD, puedes contacatrme.

¡Estaré feliz de ayudarte!
