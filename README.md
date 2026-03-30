<h1>🏨 Pagina de Booking</h1>

<p>
Aplicación web fullstack de reservas que simula una plataforma tipo booking,
permitiendo a los usuarios explorar propiedades, realizar búsquedas y gestionar reservas,
mientras que un panel de administración permite controlar el sistema internamente.
</p>

<hr>

<h2>🚀 Descripción</h2>

<p>
Este proyecto fue desarrollado como una aplicación completa separando responsabilidades en tres capas principales:
<strong>Frontend (cliente)</strong>, <strong>Backend (API)</strong> y <strong>Panel de Administración</strong>.
</p>

<p>
El objetivo es replicar el funcionamiento de una plataforma real de reservas,
aplicando buenas prácticas de desarrollo, arquitectura escalable y manejo de estado.
</p>

<hr>

<h2>🏗️ Arquitectura</h2>

<p>El proyecto está dividido en tres partes principales:</p>

<ul>
  <li><strong>Client:</strong> Interfaz pública para los usuarios</li>
  <li><strong>Admin:</strong> Panel interno de administración</li>
  <li><strong>API:</strong> Backend encargado de la lógica y los datos</li>
</ul>

<hr>

<h2>📂 Estructura del Proyecto</h2>

<pre>
📁 Pagina-de-Booking
├── 📁 admin                → Panel de administración (React + SCSS)
│   ├── public
│   │   └── index.html
│   ├── src
│   │   ├── components     → Componentes reutilizables (JSX + SCSS)
│   │   │   ├── chart
│   │   │   ├── datatable
│   │   │   ├── featured
│   │   │   ├── navbar
│   │   │   ├── sidebar
│   │   │   ├── table
│   │   │   └── widget
│   │   │      (cada carpeta contiene: componente.jsx + estilos.scss)
│   │   │
│   │   ├── context        → Manejo de estado global
│   │   │   ├── AuthContext.js
│   │   │   ├── darkModeContext.js
│   │   │   └── darkModeReducer.js
│   │   │
│   │   ├── hooks
│   │   │   └── useFetch.js
│   │   │
│   │   ├── pages          → Vistas principales (JSX + SCSS)
│   │   │   ├── home
│   │   │   ├── list
│   │   │   ├── login
│   │   │   ├── new
│   │   │   ├── newHotel
│   │   │   ├── newRoom
│   │   │   └── single
│   │   │      (cada carpeta contiene: página.jsx + estilos.scss)
│   │   │
│   │   ├── style
│   │   │   └── dark.scss
│   │   │
│   │   ├── App.js
│   │   ├── datatableSource.js
│   │   ├── formSource.js
│   │   └── index.js
│   └── package.json
│
├── 📁 api                  → Backend (Node.js + Express)
│   ├── controllers        → Lógica de negocio
│   │   ├── auth.js
│   │   ├── hotel.js
│   │   ├── room.js
│   │   └── user.js
│   │
│   ├── models             → Modelos de datos
│   │   ├── Hotel.js
│   │   ├── Room.js
│   │   └── User.js
│   │
│   ├── routes             → Endpoints de la API
│   │   ├── auth.js
│   │   ├── hotels.js
│   │   ├── rooms.js
│   │   └── users.js
│   │
│   ├── utils              → Funciones auxiliares
│   │   ├── error.js
│   │   └── verifyToken.js
│   │
│   ├── .env
│   ├── index.js
│   └── package.json
│
├── 📁 client               → Frontend (React + CSS)
│   ├── public
│   │   └── index.html
│   │
│   ├── src
│   │   ├── components     → Componentes UI (JSX + CSS)
│   │   │   ├── featured
│   │   │   ├── featuredProperties
│   │   │   ├── footer
│   │   │   ├── header
│   │   │   ├── mailList
│   │   │   ├── navbar
│   │   │   ├── propertyList
│   │   │   ├── reserve
│   │   │   └── searchItem
│   │   │      (cada carpeta contiene: componente.jsx + estilos.css)
│   │   │
│   │   ├── context        → Estado global
│   │   │   ├── AuthContext.js
│   │   │   └── SearchContext.js
│   │   │
│   │   ├── hooks
│   │   │   └── useFetch.js
│   │   │
│   │   ├── pages          → Vistas principales (JSX + CSS)
│   │   │   ├── home
│   │   │   ├── hotel
│   │   │   ├── list
│   │   │   └── login
│   │   │      (cada carpeta contiene: página.jsx + estilos.css)
│   │   │
│   │   ├── App.js
│   │   └── index.js
│   │
│   └── package.json
</pre>

<hr>

<h2>🛠️ Tecnologías</h2>

<ul>
  <li>React.js</li>
  <li>Node.js</li>
  <li>Express</li>
  <li>JavaScript (ES6+)</li>
  <li>SCSS / CSS</li>
</ul>

<hr>

<h2>⚙️ Funcionalidades</h2>

<ul>
  <li>🔍 Búsqueda de propiedades</li>
  <li>🏨 Visualización de hoteles y habitaciones</li>
  <li>📅 Sistema de reservas</li>
  <li>🔐 Autenticación de usuarios</li>
  <li>🛠️ Panel de administración para gestión de datos</li>
</ul>

<hr>

<h2>⚙️ Cómo ejecutar el proyecto</h2>

<p>Para correr este proyecto en tu entorno local, seguí estos pasos:</p>

<h3>1. Clonar el repositorio</h3>
<pre>git clone https://github.com/L0FA/Pagina-de-Booking.git</pre>

<h3>2. Backend (API)</h3>
<pre>
cd api
npm install
npm start
</pre>
<p>El servidor se ejecutará en el puerto configurado en el archivo <code>.env</code>.</p>

<h3>3. Frontend (Client)</h3>
<pre>
cd client
npm install
npm start
</pre>
<p>La aplicación se abrirá automáticamente en el navegador.</p>

<h3>4. Panel de Administración (Admin)</h3>
<pre>
cd admin
npm install
npm start
</pre>
<p>El panel de administración se ejecuta como una aplicación independiente.</p>

<h3>⚠️ Notas</h3>
<ul>
  <li>Asegurate de tener instalado <strong>Node.js</strong> y <strong>npm</strong>.</li>
  <li>Configurá correctamente las variables de entorno en el archivo <code>.env</code> dentro de la carpeta <code>api</code>.</li>
  <li>El backend debe estar corriendo para que el frontend y el admin funcionen correctamente.</li>
</ul>

<hr>

<h2>🚧 Estado del Proyecto</h2>

<p>
Proyecto en desarrollo con posibilidad de expansión hacia funcionalidades más complejas
como pagos online, dashboards analíticos y despliegue en producción.
</p>

<hr>

<h2>👤 Autor</h2>

<p>
<strong>Santiago López Fabbri</strong><br>
💻 Full Stack Developer<br>
</p>
