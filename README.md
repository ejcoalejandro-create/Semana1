Tueste Norte — Web del tostadero

Landing page para Tueste Norte, un tostadero pequeño de café de especialidad. El sitio presenta el negocio, los cafés de origen, las catas mensuales, la futura suscripción de café a domicilio y permite a los clientes escribir a través de un formulario de contacto validado en el servidor.

Herramientas utilizadas

-Visual Studio Code: como editor para todo el código (HTML, CSS, JS y PHP).
- IA: como apoyo puntual durante el desarrollo: generación de fragmentos de código, revisión de la validación en PHP. Todo el código generado ha sido revisado y entendido antes de incluirlo en el proyecto.
- XAMPP (Apache + PHP) como servidor local. 
- GitHub: para alojar el repositorio del proyecto.

Estructura del proyecto y por qué existe cada archivo

1.	index.html: Página principal (landing). Información del tostadero (los 4 cafés de origen, las catas mensuales, la suscripción y el acceso a contacto). 
2.	ficha-cata.css: Hoja de estilos única, compartida por todas las páginas, para que el diseño (colores, tipografía, formularios, botones) sea consistente en todo el sitio y no haya que repetir CSS en cada archivo.
3.	script.js: controla mostrar/ocultar los detalles de la próxima cata y el aviso de interés en la suscripción. Va en fichero aparte (no incrustado en el HTML) para mantener el contenido y el comportamiento separados.
4.	Cata.html: Formulario para reservar plaza en la cata mensual (nombre y número de plazas).
5.	Cata.php: valida los datos en el servidor y confirma la reserva o muestra los errores.
6.	contacto.html: Formulario de contacto general (nombre, email y mensaje), pedido explícitamente por el cliente para no perder recados. 
7.	contacto.php: valida en el servidor que el nombre y el mensaje no estén vacíos y que el email tenga un formato correcto, y responde con un mensaje de agradecimiento o con la lista de errores. 
8.	conversor.html / conversor.js: Herramienta interna para calcular el precio por kilo a partir del precio de un paquete de 250 g. Se enlaza de forma discreta desde el pie de página.
9.	README.md: Fundamento del proyecto. 

Los formularios Cata.html / Cata.php y contacto.html / contacto.php, se envían con method="POST"` a un script PHP porque la validación se hace en el servidor, no solo en el navegador. 

Cómo arrancarlo en local con XAMPP

Sigue estos pasos aunque no hayas visto el proyecto antes.

1. Requisitos

- Tener XAMPP (https://www.apachefriends.org/) instalado, con el módulo Apache
 
2. Coloca la carpeta del proyecto dentro de htdocs, para este proyecto queda de la siguiente manera:

C:\xampp\htdocs\Semana1\
├── index.html
├── ficha-cata.css
├── script.js
├── Cata.html
├── Cata.php
├── contacto.html
├── contacto.php
├── conversor.html
├── conversor.js
└── README.md



3. Arranca Apache

Abre el XAMPP Control Panel y pulsa Start  en la fila de Apache. Tiene que quedar en verde. 

4. Abre el sitio por localhost

En el navegador, entra en: http://localhost/Semana1/index.html (cambia “Semana1” por el nombre real de tu carpeta dentro de “htdocs”).

5. Comprueba que se ve bien en móvil

Con la página abierta, estrecha la ventana del navegador poco a poco, o abre las herramientas de desarrollador (F12) y activa el modo de dispositivo móvil (icono de móvil/tablet arriba a la izquierda del panel). 

6. Repositorio

El código está también disponible en GitHub para su seguimiento y control de
versiones: https://github.com/ejcoalejandro-create/Semana1.
