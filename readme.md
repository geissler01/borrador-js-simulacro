¡Perfecto! Te hago un **README completo**, primero en **español** y luego en **inglés**, listo para colocar en tu proyecto. Lo estructuré como un README profesional de proyecto de frontend con JSON Server.

---

# 📄 README (Español)

```markdown
# Proyecto Demo: CRUD de Cartas de Comida con Login y Sesión

Este proyecto es un **borrador funcional offline** que simula un sistema de login y un CRUD de cartas de comida utilizando **JSON Server** como backend falso. Está pensado para **pruebas técnicas y desarrollo local**.

---

## 🗂 Estructura del proyecto

```

/project
│
├── db.json            <-- Base de datos JSON
├── login.html         <-- Página de login
├── landing.html       <-- Página de usuario
├── admin.html         <-- Panel de administración
│
├── login.js           <-- Lógica de login
├── landing.js         <-- Render y modal de cartas en landing
├── admin.js           <-- CRUD completo con tabla de cartas

````

---

## ⚡ Requisitos

- Node.js (para instalar JSON Server)
- Navegador moderno (Chrome, Firefox, etc.)
- Conexión local a `localhost:3000` (JSON Server)

---

## 🚀 Instrucciones de instalación

1. Instalar JSON Server globalmente:

```bash
npm install -g json-server
````

2. Levantar el servidor falso:

```bash
json-server --watch db.json --port 3000
```

3. Abrir `login.html` en el navegador.

---

## 👤 Usuarios de prueba

| Email                                   | Password | Rol   |
| --------------------------------------- | -------- | ----- |
| [admin@mail.com](mailto:admin@mail.com) | 123      | admin |
| [user@mail.com](mailto:user@mail.com)   | 123      | user  |

---

## 📝 Funcionalidades

### Login

* Valida usuario y contraseña contra `/users`.
* Guarda sesión en `localStorage` (`isAuth`, `role`, `currentUser`).
* Redirige a `admin.html` o `landing.html` según rol.

### Landing (Usuario)

* Muestra cartas de comida desde `/foods`.
* Modal de Bootstrap para ver detalles (imagen, nombre, descripción, precio).
* Solo accesible si `role=user` y sesión activa.

### Admin

* CRUD completo de cartas de comida:

  * **Crear:** mediante inputs o modal.
  * **Editar:** modificar campos específicos con `PATCH`.
  * **Eliminar:** elimina carta seleccionada.
* Tabla interactiva que refleja cambios en tiempo real.
* Solo accesible si `role=admin` y sesión activa.

---

## 💻 Tecnologías utilizadas

* HTML5 / CSS3 / Bootstrap 5
* JavaScript (ES6, async/await, fetch)
* JSON Server (backend falso)
* LocalStorage (gestión de sesión)

---

## 🛠 Notas

* Modal en landing es solo para **visualizar** cartas.
* Modal en admin puede implementarse para **crear/editar** cartas.
* Persistencia de sesión se mantiene mientras exista `localStorage`.
* Seguridad básica: no se puede acceder a páginas sin sesión ni rol correcto.

---

## 📝 Observaciones

Este proyecto es **educativo**, orientado a pruebas offline y flujo completo de CRUD + login, listo para expandirse a backend real si se desea.

````

---

# 📄 README (English)

```markdown
# Demo Project: Food Cards CRUD with Login and Session

This project is a **functional offline draft** simulating a login system and a CRUD for food cards using **JSON Server** as a fake backend. It is designed for **technical tests and local development**.

---

## 🗂 Project Structure

````

/project
│
├── db.json            <-- JSON database
├── login.html         <-- Login page
├── landing.html       <-- User page
├── admin.html         <-- Admin panel
│
├── login.js           <-- Login logic
├── landing.js         <-- Rendering and modal for cards
├── admin.js           <-- Full CRUD with table

````

---

## ⚡ Requirements

- Node.js (to install JSON Server)
- Modern browser (Chrome, Firefox, etc.)
- Local connection to `localhost:3000` (JSON Server)

---

## 🚀 Installation

1. Install JSON Server globally:

```bash
npm install -g json-server
````

2. Run the fake server:

```bash
json-server --watch db.json --port 3000
```

3. Open `login.html` in the browser.

---

## 👤 Test Users

| Email                                   | Password | Role  |
| --------------------------------------- | -------- | ----- |
| [admin@mail.com](mailto:admin@mail.com) | 123      | admin |
| [user@mail.com](mailto:user@mail.com)   | 123      | user  |

---

## 📝 Features

### Login

* Validates email and password against `/users`.
* Stores session in `localStorage` (`isAuth`, `role`, `currentUser`).
* Redirects to `admin.html` or `landing.html` according to role.

### Landing (User)

* Displays food cards from `/foods`.
* Bootstrap modal to view details (image, name, description, price).
* Accessible only if `role=user` and session active.

### Admin

* Full CRUD for food cards:

  * **Create:** using inputs or modal.
  * **Edit:** modify specific fields using `PATCH`.
  * **Delete:** remove selected card.
* Interactive table reflecting changes in real-time.
* Accessible only if `role=admin` and session active.

---

## 💻 Technologies Used

* HTML5 / CSS3 / Bootstrap 5
* JavaScript (ES6, async/await, fetch)
* JSON Server (fake backend)
* LocalStorage (session management)

---

## 🛠 Notes

* Landing modal is only for **viewing** cards.
* Admin modal can be implemented for **create/edit** cards.
* Session persistence works while `localStorage` exists.
* Basic security: cannot access pages without correct role/session.

---

## 📝 Remarks

This project is **educational**, suitable for offline testing and demonstrating a full CRUD + login flow, ready to expand to a real backend if needed.

```

---

Si quieres, puedo hacer **una versión extendida** donde además del README se agregue **instrucciones de cómo usar modales en admin para crear y editar cartas**, dejando todo profesional y listo para entregar en un portafolio.  

¿Quieres que haga eso también?
```
