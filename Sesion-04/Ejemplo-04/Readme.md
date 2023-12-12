[`Introducción a Bases de Datos`](../../Readme.md) > [`Sesión 04`](../Readme.md) > Ejemplo 4

## Ejemplo 4: Configuración de __MongoDB__ en la nube

### 1. Objetivos :dart:
- Que el alumno configure MongoDB en la nube

### 2. Requisitos :clipboard:
- Ninguno

### 3. Desarrollo :rocket:
1. Para poder hacer uso de MongoDB en la nube se hará uso del servicio __Atlas__ proveeido por el propio equipo de MongoDB, abrir la siguiente url, llenar los campos del formulario, y dar clic en el botón de __Create your Atlas account__

   URL: https://www.mongodb.com/cloud/atlas/register

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/a375fb4a-08dc-4afe-b6e6-4e2c13526268)

1. Te mandará un correo de verificación.

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/f371bc9b-122d-4423-8a12-d72937b1baf2)

1. Es necesario ingresar a tu cuenta de correo y abrir el correo de __MongoDB Cloud__ y dar clic en __Verify Email__

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/65598d96-30f2-4dee-af5b-22ad808a5cbe)

1. Posteriormente en la página que se abre dar clic en __Continue__

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/25bc3b07-b2e1-46d6-b145-9a9b287f27bd)

1. Llenar el siguiente formulario seleccionando las opciones y dar clic en __Finish__:
   * Learn MongoDB
   * New to MongoDB
   * Other
   * Other
   * Not sure

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/47fe6067-cb85-4875-b4bf-36ed2ad0c8c0)

1. Elegir el tipo de __Cluster__, en donde se seleccionará __M0 FREE__ que es el que es libre de costo, dejar todas las opciones como vienen por defecto, dar clic en el botón __Create__.

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/5ed4917d-d7e7-4efd-bf77-3a890f0b531e)

   Observar que con MongoDB Atlas se crean __Clusters__ y no __Servidores__.

   Cuando el __Cluster__ ya está creado se observa la página como la siguiente:

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/06f86cbc-fa5d-4a47-9eda-af1712b874ae)

1. Lo que sigue es crear una conexión al cluster de MongoDB en la nube
   Introduce los datos que desees para ingresar a tu base de datos, __por ejemplo__:

   - Usuario: mongouser
   - Password: mongouser1234 (Puedes usar el Autogenerador de Password Seguro)
   
   **Recuerda el vídeo de contraseñas seguras `mongouser1234` no es una contraseña muy segura que digamos...**  
   
   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/06c2a846-6964-4f0f-9fa4-1dbfedb09bfc)
   
   **Guarda la contraseña en un sitio seguro porque es la que utilizarás para conectarte al cluster**  
   **__Nota:__ No uses los datos del ejemplo para colocar información sensible.**

   Y presionar en el botón __Create User__

   Se agregará el usuario a la lista de usuarios

   MongoDB Atlas hace una validación y solicita definir que dirección IP se va a conectar a el servidor y que usuario.
   
   Así que dá clic en el botón __Add My Current IP Address__

   En la lista aparecerá tu IP con la descripcion "My IP Address"
   
   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/64f1dc9f-8119-4a3c-896b-af8fb41832f5)
  
   Si te conectas desde varios lugares diferentes se sugiere etiquetar la dirección IP, para llevar un registro de a quién corresponde cada IP y más adelante poder eliminar las direcciones que ya no sean necesarias.
  
   Y posteriormente se dá clic en el botón __Finish and Close__

1. En la ventana que aparece das clic en __Go to Overview__

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/4a89ddfa-7bbd-4893-a473-2f1a5b87c159)

1. Para obtener la cadena de conexion das clic en el boton __Conect__ donde se seleccionará __Compass__ para continuar en el siguiente ejemplo.

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/fd58656b-a755-4a1b-99e3-91a0576d3aaa)
   
   Seleccionas la opcion __I have MongoDB Compass installed__ para que te muestre la cadena de conexion. Copia la __connection string__ y pegalo en un block de notas, donde deberás reemplazar el texto __<password>__ por el password asignado al usuario que creaste en el paso anterior.

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/ca19f011-b163-4a47-ab23-12e08fc3dfdd)

1. Si __MongoDB Compass__ está abierto es necesario cerrarlo y abrirlo nuevamente, la ventana inicial solicita la cadena de conexión, en donde debes pegar la cadena de conexion que obtuviste en el paso anterior:

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/7a9e4d22-2183-49d0-8a78-2415164a525d)

   En este punto ya __Compass__ ya estará conectado al __Cluster0__ que como se puede ver en la columna izquierda consta de 3 instancias de MongoDB corriendo en paralelo lo que se puede escalar según las necesidades.

   ![image](https://github.com/AlonsoElesbaan/Introduccion-a-Bases-de-Datos-Diciembre-2020/assets/83846645/11609763-45ad-4e26-8b8b-6944fbcfa1fa)

[`Anterior`](../Readme.md#configuración-de-mongodb-en-la-nube) | [`Siguiente`](../Readme.md#operaciones-con-bases-de-datos-1)   
