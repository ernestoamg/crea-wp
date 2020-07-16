# crea-wp

Este script depende del usuario root.

Crea una instancia de WordPress utilizando WP-cli
Este código toma partes de https://gist.github.com/rjekic/2d04423bd167f8e7afd26f8982609378 y elimina la opción de hacer una instalación utilizando comandos del sistema operativo y se basa unicamente en wp-cli.

Es script realiza las siguientes tareas:

- Crea la carpeta de donde se va a descargar a instalar el WordPress
- Crea una base de datos con los datos provistos
- Crea el usuario de la base de datos y le da privilegios
- Instala wp-cli para poder utilizarlo
- Descarga WordPress en su versión más reciente (en español)
- Crea un archivo wp-config usando las credenciales definidas
- Instala el sitio de Wordpress usando las credenciales definidas
- Permite asignar un nuevo prefijo de las tablas para la base de datos
- Ejecuta acciones para limpiar instalaciones de temas/plugins que vienen por default en WP
- Instala plugins que requiero en mi instalación nueva
- Elimina los pots y páginas por default de WordPress
- Realiza ajustes de parámetros default necesarios como timezone y permalinks
- Genera el archivo .htaccess
- Permite asignar a mis carpetas y archivos, el nombre de usuario y grupo requeridos


Pendientes:
- Eliminar la dependencia del usuario root y ejecutar como el usuario que instala la instancia.
- Cambiar de vuelta los privilegios elevados al usuario en la base de datos.
- Agregar otros plugins a la lista por default.
- Asegurar mejor la instancia con reglas específicas en el archivo .htaccess
- Crear un archivo de parámetros con la receta de la instancia a crear.
