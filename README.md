# Mr. Barber - Reservation System

## Executive Summary

### Description
Mr. Barber is a web application designed to facilitate appointment management in a barbershop.
It allows customers to create accounts, schedule appointments, modify details, and view their history. 
The solution aims to prevent appointment mix-ups and provide an efficient experience for both customer and staff.

### Identified Problem
The barbershop owner mentioned issues with appointment management such as mixed reservations and difficult answering calls without a secretary. A solution was sought to simplify scheduling and improve organization.

### Solution
The implemented solution is a web page that allows customers to create accounts, schedule appointments, modify details and cancel reservations. Additionally, an admin system provides access to view future and same-day appointments.

### Architecture 
The application uses MongoDB Compass as the database to store services and appointments. It was developed in JavaScript (Node.js v18.17.0) and structured with Express.js for the backend and Tailwind CSS for the frontend.

### Table of Contents
1. [Requirements](#Requirements)
2. [Installation](#Installation)
3. [Configuration](#Configuration)
4. [Usage](#Usage)
5. [Contribution](#Contribution)
6. [Reference Manual](#ReferenceManual)

### Requirements
- Application Servers: Node.js (v18.17.0)
- Database: MongoDB Compass
- PostCSS, Autoprefixer

### Installation
1. Download and install MongoDB Compass and connect to the database using the URL provided privately.
2. Clone the repository using GitHub Desktop.
3. Open the frontend folder and create a ".env.local" file with the required path variable provided privately.
4. Open a terminal and access the backend folder:
- cd /Mr.Barber/backend
- npm install
- npm install mongoose
   - npm install express
   - npm i -D nodemon
   - npm install dotenv
   - npm uninstall bcrypt
   - npm install bcrypt
   After this installations, run the backend as follows:
   - npm run dev:postman
5. Open a new terminal and access the frontend folder:
   - cd /Mr.Barber/frontend
   - npm i -D tailwindcss postcss autoprefixer
   - npx tailwindcss init -p
   After these installations, run the frontend as follows:
   - npm run dev
To run the tests manually, just follow the steps as if you were creating new appointments.

### Configuration
- Product Configuration: Configuration files in the frontend and backend folder.
- Requirement Configuration: Settings in the database and the ".env.local" file.

### Contribution
Steps to contribute
1. Clone the repository using GitHub Desktop.
2. Create a new branch or select an existing one.
3. Make changes and commit to the created branch.
4. Submit a Pull Request and wait for the team review.
5. Merge into the master branch

## Reference Manual
### End User
#### Create Account
1. Fill out the registration form.
2. Click "Crear Cuenta".
3. Receive a confirmation email.
4. Open the email and click the URL to verify your account.

#### Log In
1. Access the Mr. Barber website.
2. On the homepage, enter your verified account credentials.
3. Click the "Iniciar Sesión" button.
4. You will be redirected to the homepage where you can view your appointments.

#### Create Appointment
1. Click the "Nueva Cita" button.
2. Select a maximum of 2 services.
3. Click the "Detalles de la cita" button.
4. Scroll down and select an available date and time.
5. Click the "Confirmar Reservación" button.
6. You will be redirected to the homepage where you can view your appointments.

#### Modify Appointment
1. Click the "Modificar Cita" button.
2. Select services to change, if desired. If not, click the "Detalles de la cita" button.
3. Select the new time or date.
4. Click the "Confirmación Reservación".
5. You will receive a confirmation email.

#### Cancel Appointment
1. Click the "Cancelar Cita" button.
2. Confirm the cancellation message.
3. You will receive a confirmation email.

#### Recover Password
1. If you forgot your password, click the "Crear contraseña" button.
2. Enter the email address for the account you forgot the password for.
3. You will receive an email with a link to change your password.
4. Follow the link and change your password.

### Administrator User
#### Access as Admin
1. Create an account as a normal user.
2. Access MongoDB Compass and change the boolean variable for your account to make it an admin.

#### Admin Features
1. View future or same-day appointments on the main page.
2. Cannot modify or cancel appointments made by regular users.
3. Access the database to perform administrative operations.


# Mr. Barber - Sistema de Reservaciones

## Resumen Ejecutivo

### Descripción
Mr. Barber es una aplicación web diseñada para facilitar la gestión de citas en una barbería. 
Permite a los clientes crear cuentas, programar citas, modificar detalles y visualizar su historial.
La solución busca evitar confusiones en las citas y brindar una experience eficiente tanto para los clientes
como para el personal.

### Problema identificado
La dueña de la barbería mencionó problemas con le gestión de las citas, como la mezcla de reservaciones
y la dificultad para recibir llamadas en ausencia de una secretaria. Se buscó una solución que facilitara
la programación de citas y mejorara la organización.

### Solución
La solución implementada es una página web que permite a los clientes crear cuentas, programar citas, 
modificar detalles y cancelar reservaciones. Además, un sistema de adminsitrador que proporciona acceso 
a la visualización de citas futuras y del día.

### Arquitectura
La aplicación utiliza una base de datos MongoDB Compass para almacenar servicios y citas. Se desarrolló 
en JavaScript (Node.js v18.17.0) y se estructuró con Express.js para el backend y Tailwind CSS
para el frontend.

### Tabla de Contenidos 
1. [Requerimientos](#Requerimientos)
2. [Instalación](#Instalación)
3. [Configuración](#Configuración)
4. [Uso](#Uso)
5. [Contribución](#Contribución)
6. [Manual de Referencia](#ManualdeReferencia)

### Requerimientos
- Servidores de aplicación: Node.js (v18.17.0)
- Base de datos: MongoDB Compass
- PostCSS, Autoprefixer

### Instalación
1. Descargar e instalar MongoDB Compass y conectarse a la base de datos con la URL proporcionada por
privado.
2. Clonar el repositorio utilizando GitHub Desktop.
3. Abrir la carpeta del frontend y crear un archivo '.env.local' con la variable de ruta necesaria proporcionada
de igual manera por privado.
4. Abrir una terminal y acceder a la carpeta del backend
   - cd /Mr.Barber/backend
   - npm install
   - npm install mongoose
   - npm install express
   - npm i -D nodemon
   - npm install dotenv
   - npm uninstall bcrypt
   - npm install bcrypt
   Una vez hechas estas instalaciones se corre el backend de la siguiente manera. 
   - npm run dev:postman
5. Abrir una terminal nueva y acceder a la carpeta del frontend
   - cd /Mr.Barber/frontend
   - npm i -D tailwindcss postcss autoprefixer
   - npx tailwindcss init -p
   Una vez hechas estas instalaciones se corre el frontend de la siguiente manera.
   - npm run dev

Para ejecutar las prubeas manualmente solo se seguiran los pasos como si se fuese a crear nuevas citas. 


### Configuración
- Configuración del producto: Archivos de configuración en la carpeta del frontend y backend
- Configuración de requerimientos: Ajustes en la base de datos y en el archivo '.env.local'

### Contribución
#### Pasos para contribuir
1. Clonar el repositorio usando GitHub Desktop.
2. Crear una nueva rama o seleccionar una existente.
3. Realizar cambios y hacer commit en la rama creada.
4. Enviar un Pull Request y esperar la revisión del equipo.
5. Realizar el merge en la rama master.

## Manual de Referencia
### Usuario Final
#### Crear cuenta
1. Llenar el formato de registro.
2. Haz clic en "Crear Cuenta".
3. Recibir correo de confirmación.
4. Abrir el correo y hacer clic en la URL para verificar tu cuenta.
   
#### Iniciar Sesión
1. Accede a la página web de Mr. Barber
2. En la página de inicio, introduce tus credenciales de cuenta verificada.
3. Haz clic en el botón "Iniciar Sesión".
4. Redirrecciona a página de inicio donde podrás visualizar tus citas.

#### Crear Cita
1. Haz clic en el botón "Nueva Cita".
2. Seleccionar un máximo de 2 servicios.
3. Haz clic en el botón "Detalles de la cita"
4. Scroll hacia abajo y seleccionar fecha y hora disponible.
5. Haz clic en el botón "Confirmar Reservación".
6. Redirrecciona a página de inicio donde podrás visualizar tus citas.

#### Modificar Cita
1. Haz clic en el botón "Modificar Cita"
2. Seleccionar servicios a cambiar, si es lo que se desea. Si no, haz clic en el botón "Detalles de la cita".
3. Seleccionar el cambio de hora o fecha.
4. Haz clic en el bóton [Confirmación Reservación".
5. Recibir correo de confirmación.

#### Cancelar Cita
1. Haz clic en el botón "Cancelar Cita".
2. Confirmar el mensaje de cancelación.
3. Recibir correo de confirmación.

#### Recuperar Contraseña
1. Si olvidaste tu contraseña, haz clic en el botón de crear contraseña.
2. Ingresa tu correo electrónico de la cuenta que olvidaste la contraseña.
3. Recibirás un correo con un enlance de cambiar tu contraseña.
4. Sigue el enlace y realiza el cambio de contraseña.

### Usuario Administrador
#### Acceso como Administrador
1. Crea una cuenta como usuario normal.
2. Accede a MongoDB Compass y cambia la variable booleana correspondiente a tu cuenta para convertirla en administrador.

#### Funcionalidades del Administrador
1. Visualizar las citas futuras o del día en la página principal.
2. No puede modificar ni cancelar citas de usuarios normales.
3. Accede a la base de datos para realizar operaciones administrativas.

 
