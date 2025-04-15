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

## Cómo comenzar

### 1. Clona este repositorio

---(En tu terminal)

```git clone https://github.com/RamonMartinez01/Node.js-Express-Starter-01.git```

---una vez clonado entra a la carpeta raíz del proyecto

```cd Node.js-Express-Starter-01```

### 2. Instala las dependencias
  ```npm install```

### 3. Configura tus variables de entorno
---Copia el archivo de ejemplo .env.example y crea uno nuevo (puedes usar este comando):
 
  ```cp .env.example .env```

---Asegúrate de que tu base de datos esté creada y corriendo en PostgreSQL (-No necesitas hacer nada con la base de datos por ahora, solo crearla).

---Abre el archivo .env y reemplaza <nombre_db> por el nombre real de tu base de datos:

    ```DATABASE_URL=postgres://postgres:tu_contraseña@127.0.0.1:5432/nombre_real_de_tu_db```

### 4. Ejecuta el proyecto
---En desarrollo (con reinicios automáticos):

  ```npm run dev```

---En producción:

  ```npm start```
  
* Esto quiere decir que mientras estés trabajando en tu computadora (modo desarrollo), 
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

### ¿Por qué usar esta plantilla?

Porque te ahorra tiempo configurando lo básico y te permite enfocarte en desarrollar tu API sin preocuparte por la estructura inicial.
Ideal para prácticas, proyectos personales o incluso pruebas técnicas.

### ¿Tienes dudas?

No dudes en abrir un Issue en este repositorio, agregarme como colaborador a tu nuevo repositorio o contactarme por correo ```beehiverm@gmail.com```.
¡Estaré feliz de ayudarte!
