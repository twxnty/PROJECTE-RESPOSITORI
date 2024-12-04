TwentyOS - Sistema Operativo Simulado
TwentyOS es un sistema operativo simulado, diseñado para funcionar en una interfaz de consola de texto. Su objetivo es proporcionar una experiencia interactiva simple para realizar operaciones básicas de sistema, gestión de archivos, cálculos, y más, todo en un entorno de consola. El sistema está implementado en C# y está pensado para ser una herramienta de aprendizaje o una base para el desarrollo de proyectos más complejos.

Funcionalidades Principales
Comandos del Sistema
TwentyOS se maneja mediante una serie de comandos que el usuario puede ejecutar desde la terminal. A continuación, se describen los comandos disponibles:

1. about
Muestra información general sobre el sistema operativo, como su versión y una breve descripción de su funcionalidad.

2. shutdown
Apaga el sistema operativo de manera simulada, mostrando un mensaje de "apagado" en la consola.

3. reboot
Reinicia el sistema operativo simulado. Tras ejecutar el comando, el sistema se reiniciará y mostrará nuevamente el menú principal.

4. help
Muestra el listado completo de comandos disponibles, junto con una breve descripción de cada uno.

5. calculadora
Accede a una calculadora básica, donde puedes realizar operaciones matemáticas entre dos números.

6. ls
Lista el contenido del directorio actual. Este comando simula el comportamiento de la herramienta ls en sistemas UNIX, mostrando los archivos y carpetas del directorio activo.

7. mkfile
Permite crear un archivo en el sistema de archivos. El usuario debe proporcionar un nombre para el archivo y su contenido.

8. writefile
Escribe texto en un archivo existente. Si el archivo no existe, el comando lo creará automáticamente.

9. readfile
Lee y muestra el contenido de un archivo especificado por el usuario.

Requisitos del Sistema
Para ejecutar TwentyOS en tu máquina, necesitarás tener instalada la plataforma .NET Core. El proyecto ha sido desarrollado con .NET 6.0, por lo que se recomienda usar esta versión o superior.

.NET 6.0 o superior: Puedes descargarlo desde aquí.
Sistema operativo: Compatible con Windows, macOS y Linux.
Terminal o consola compatible con caracteres ASCII.
Instalación y Ejecución
1. Clonar el repositorio
Para comenzar a usar TwentyOS, clona este repositorio en tu máquina local:

bash
Copiar código
git clone https://github.com/tu-usuario/twentyos.git
cd twentyos
2. Restaurar dependencias
Si es la primera vez que descargas el proyecto, asegúrate de restaurar las dependencias del proyecto utilizando el siguiente comando:

bash
Copiar código
dotnet restore
3. Ejecutar el proyecto
Una vez restauradas las dependencias, puedes ejecutar el proyecto con:

bash
Copiar código
dotnet run
4. Interactuar con el sistema
Una vez que el sistema esté en ejecución, puedes empezar a interactuar con el mismo mediante los comandos mencionados anteriormente.

Estructura del Proyecto
El código fuente está organizado en varias clases y métodos que permiten gestionar la interacción del usuario con el sistema. A continuación se describe brevemente la estructura de algunas de las clases clave:

Program.cs: Es el punto de entrada principal del sistema operativo. Aquí se gestionan la ejecución de comandos y la presentación del menú.
Comandos.cs: Contiene la lógica para ejecutar los comandos disponibles, como crear archivos, escribir en ellos, y realizar cálculos.
Sistema.cs: Simula las funciones de gestión del sistema, como apagar o reiniciar el sistema.
Interfaz.cs: Gestiona la interacción visual con el usuario, incluyendo la presentación del menú y la salida de texto.
Métodos Principales
MostrarMenuPrincipal(): Muestra el menú principal con el título de TwentyOS y las opciones de comandos disponibles.
ElegirOpcion(string text): Procesa la opción seleccionada por el usuario.
CreateFile(): Permite crear un archivo en el sistema. El usuario debe proporcionar un nombre y contenido para el archivo.
WriteFile(): Escribe contenido en un archivo previamente creado.
ReadFile(): Muestra el contenido de un archivo.
ListFiles(): Lista los archivos presentes en el directorio actual simulado.
ShowAbout(): Muestra una breve descripción de TwentyOS.
shutdownSystem(): Apaga el sistema operativo simulado.
rebootSystem(): Reinicia el sistema operativo.
Ejemplos de Uso
Comando about
Al ejecutar el comando about, el sistema mostrará información sobre TwentyOS:

bash
Copiar código
about
Salida esperada:

arduino
Copiar código
TwentyOS v1.0 - Sistema Operativo Simulado.
Desarrollado en C# para propósitos educativos.
Comando calculadora
Al ejecutar el comando calculadora, el sistema pedirá que ingreses dos números y una operación para realizar el cálculo:

bash
Copiar código
calculadora
Entrada esperada:

Copiar código
Introduce el primer número: 5
Introduce el segundo número: 3
Introduce la operación (+, -, *, /): +
Salida esperada:

yaml
Copiar código
El resultado es: 8
Comando ls
Al ejecutar el comando ls, se listarán los archivos en el directorio actual:

bash
Copiar código
ls
Salida esperada:

Copiar código
file1.txt
file2.txt
folder1/
folder2/
Comando mkfile
Este comando te permite crear un archivo. Primero, se solicita el nombre del archivo y luego el contenido:

bash
Copiar código
mkfile
Entrada esperada:

less
Copiar código
Introduce el nombre del archivo: archivo1.txt
Introduce el contenido del archivo: Este es un archivo de prueba.
Salida esperada:

arduino
Copiar código
Archivo 'archivo1.txt' creado con éxito.
Contribuciones
Las contribuciones son bienvenidas. Si deseas mejorar o agregar nuevas funcionalidades a TwentyOS, sigue estos pasos:

Haz un fork del repositorio.
Crea una nueva rama para tu funcionalidad (git checkout -b feature/nueva-funcionalidad).
Realiza tus cambios y realiza un commit (git commit -am 'Añadir nueva funcionalidad').
Sube tus cambios al repositorio remoto (git push origin feature/nueva-funcionalidad).
Abre un pull request explicando los cambios realizados.
Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.

Este README ahora ofrece una descripción más detallada de la funcionalidad, estructura y uso de TwentyOS. Además, incluye ejemplos más elaborados y la información necesaria para que otros contribuyan al proyecto. ¡Espero que te guste!
¡Esperamos que disfrutes de esta experiencia con twenOS!