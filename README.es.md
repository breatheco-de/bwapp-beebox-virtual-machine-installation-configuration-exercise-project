# Instalación de bWapp usando una Máquina Virtual (BeeBox)  

En 4Geeks Academy, estamos comprometidos a proporcionar la mejor experiencia de aprendizaje para nuestros estudiantes, especialmente en lo que respecta a la comprensión de la seguridad web. Una herramienta esencial en nuestro plan de estudios es bWAPP (Buggy Web Application), una aplicación web gratuita y de código abierto que es deliberadamente vulnerable, diseñada para ayudar a los estudiantes a aprender sobre las vulnerabilidades de seguridad web y cómo mitigarlas.

Hay dos formas principales de instalar bWAPP:
1. **Instalación Manual:** Instalando los archivos directamente en tu propio servidor LAMP (Linux, Apache, MySQL, PHP) o WAMP (Windows, Apache, MySQL, PHP).
2. **Instalación en Máquina Virtual:** Ejecutando bWAPP usando una máquina virtual preconfigurada (VM) como BeeBox.

En 4Geeks Academy, hemos elegido usar el enfoque de máquina virtual por varias razones convincentes que puedes leer al final de este artículo.

## Cómo Instalar bWAPP Usando una Máquina Virtual

Aquí están los pasos para poner en marcha bWAPP usando BeeBox:

1. **Extraer el Archivo Comprimido:**
   Descarga y extrae el [archivo de la VM de BeeBox aquí.](https://storage.googleapis.com/breathecode/virtualbox/bee-box_v1.6.7z).

2. **Crear una Nueva Máquina Virtual:**
   * Inicia VirtualBox.
   * Haz clic en Nueva.
   * Nombra la VM y especifica Linux como el tipo de sistema operativo para tu maquina. Luego deja la configuración por defecto para memoria y procesador.

3. **Configurar Almacenamiento:**
   * Ve a Configuración > Almacenamiento.
   * Añade el archivo que extrajiste en la carpeta `/beebox` con el nombre `beebox.vmdk` 


4. **Go to the bWAPP Login Page:**
   Haz click sobre `bWAPP - start` y el navegador web se abrirá. Usa las credenciales predeterminadas para iniciar sesión, o crea un nuevo usuario.

   ```
   Default credentials 
   username: bee
   password: bug
   ```

**¡Estás Listo para Explorar y Explotar bWAPP!**
   Comienza a explorar y explotar las vulnerabilidades dentro de bWAPP en un entorno seguro y controlado.

> 🔥  IMPORTANTE: Evita actualizar el sistema operativo Linux, ya que resolverá muchas de las vulnerabilidades y disminuirá la diversión.

## Notas Importantes de Instalación:
   Aunque estos pasos no son necesarios para la instalación y configuración básica de bWAPP, proporcionan información útil para mantener y personalizar el entorno, así como para llevar a cabo   actividades más avanzadas de hacking y pruebas de seguridad.

* **Credenciales de Linux::**
  ```
  bee/bug
  root/bug
  ```

* **Credenciales de MySQL:**
  ```
  root/bug
  ```

* **Modificar la Configuración de Postfix:**
  Ajusta el relayhost y otras configuraciones para que coincidan con tu entorno.
  ```
  Configuration file: /etc/postfix/main.cf
  ```

* **Defacing y Hacking:**
  BeeBox ofrece varias formas de desfigurar el sitio web de bWAPP. Incluso es posible hackear BeeBox para obtener acceso root. ¡Diviértete!

* **Tomar una Instantánea Antes de Hackear:**
  Toma una instantánea de la VM antes de comenzar tus actividades de hacking. También hay una copia de seguridad del sitio web de bWAPP disponible en `/var/www/bWAPP_BAK`.

* **Reinstalación de la Base de Datos de bWAPP:**
  Si es necesario, puedes eliminar la base de datos usando phpMyAdmin  (http://[IP]/phpmyadmin/). Luego, reinstala la base de datos de bWAPP navegando a:
  ```
  http://[IP]/bWAPP/install.php
  ```

## Los Beneficios de Usar una Máquina Virtual para Instalar bWAPP

1. **Facilidad de Uso:**
   Configurar bWAPP manualmente implica varios pasos: instalar un servidor web, configurar PHP, configurar una base de datos MySQL y resolver problemas potenciales. Esto puede llevar tiempo y ser complejo, especialmente para principiantes. En contraste, usar una VM como BeeBox es sencillo. Simplemente descargas la VM, la importas en tu software de virtualización (como VirtualBox o VMware) y la inicias. El entorno está preconfigurado y listo para usar, ahorrando tiempo y esfuerzo valiosos.

2. **Entorno Consistente:**
   Con una VM, obtienes un entorno consistente y estable. Esto elimina la variabilidad que puede ocurrir al configurar bWAPP en diferentes sistemas con diferentes configuraciones. Los estudiantes e instructores pueden estar seguros de que están trabajando en el mismo entorno, lo que facilita seguir las lecciones y solucionar cualquier problema que surja.

3. **Aislamiento y Seguridad:**
   Ejecutar bWAPP en tu propio servidor puede exponer tu computadora a vulnerabilidades de seguridad. Dado que bWAPP es intencionalmente vulnerable, cualquier mala configuración o descuido puede llevar a riesgos de seguridad. Al usar una VM, aíslas bWAPP de tu sistema operativo principal. Este aislamiento minimiza el riesgo de comprometer tus archivos personales u otras aplicaciones en tu computadora. La VM actúa como una caja de arena, conteniendo cualquier amenaza de seguridad potencial dentro del entorno virtual.

4. **Gestión de Recursos:**
   Las máquinas virtuales están diseñadas para gestionar eficientemente los recursos del sistema. Puedes asignar cantidades específicas de CPU, memoria y almacenamiento a la VM, asegurando que tu sistema operativo principal permanezca receptivo y funcional incluso mientras ejecutas aplicaciones que consumen muchos recursos como bWAPP.

5. **Portabilidad:**
   Las VM son altamente portátiles. Puedes mover fácilmente una VM de una computadora a otra, compartirla con compañeros de clase o colegas, o hacer una copia de seguridad para uso futuro. Esta portabilidad facilita mantener un entorno de desarrollo consistente en diferentes máquinas y ubicaciones.

#### Conclusión

En 4Geeks Academy, creemos en aprovechar las mejores herramientas y prácticas para mejorar nuestros programas educativos. Al usar una máquina virtual para ejecutar bWAPP, simplificamos el proceso de configuración, aseguramos un entorno de aprendizaje consistente y seguro, y protegemos nuestros sistemas de potenciales vulnerabilidades. Este enfoque no solo beneficia a nuestros estudiantes, sino que también se alinea con nuestro compromiso de ofrecer educación de alta calidad en el campo de la seguridad web.

Ya seas estudiante, educador o profesional, recomendamos encarecidamente usar el enfoque de máquina virtual para la instalación de bWAPP. Es una decisión que aporta conveniencia, seguridad y tranquilidad.