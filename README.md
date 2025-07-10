# BOMA
Prueba técnica desarrollador. 
Este proyecto contiene:

- /backend → API Node.js con Express y JWT
- /frontend → App React

Base de datos simulada con JSON local.

#INSTRUCCIONES.

1. Sobre la carpeta backend, en la ventana de comando escribir el siguiente comando: node server.js
2. Sobre la carpeta front, en la ventana de comando escribir el siguiente comando: npm start

#ENDPOINTS DEL API
1. /login
   Metodo: POST
   Seguridad: No
   Parametros:
   username (string),
   password (string)

   Respuesta:
   200 OK
   Token

3. /registroUsuarios
   Metodo: POST
   Seguridad: No
   Parametros:
    username (String),
    password (String),
    nombre (String),
    apellidoPaterno (String),
    apellidoMaterno (String),
    fechaNacimiento (DateTime),
    correo (String),
    lugarNacimiento (String)
   Repuesta:
   200 OK
 
3. /getUsuarios
   Metodo: GET
  Seguridad: Bearer Token

   Respuesta:
   200 OK
   Lista de usuarios:
   {
       username (String),
      nombre (String),
      apellidoPaterno (String),
      apellidoMaterno (String),
      fechaNacimiento (DateTime),
      correo (String),
      lugarNacimiento (String)
   }

4. /editUsuario/:id
   Metodo: PUT
   Seguridad: Bearer Token
   Parametros:
    username (String),
    password (String),
    nombre (String),
    apellidoPaterno (String),
    apellidoMaterno (String),
    fechaNacimiento (DateTime),
    correo (String),
    lugarNacimiento (String)
   Repuesta:
   200 OK

5. /deleteUsuarios/:id
  Metodo: DELETE
  Seguridad: Bearer Token
   Respuesta:
   200 OK
