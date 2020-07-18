# Sistemas Operativos(C2020-162013G2) - ULACIT

## Tabla de Contenidos
- [Bitacora de comandos](#lista-de-comandos)

## Lista de Comandos

### Comando especiales
- `sudo` es un prefijo que se asegura de ejecutar el comando con privilegios de administrador o "root".
- `apt` es el administrador de paquetes avanzado que viene disponible en muchas distribuciones de linux.

## Administracion de paquetes
|Comando|Descripcion|
| ------- | ------- |
| `sudo apt update` | Actualiza los paquetes disponibles y sus versiones, pero no actualiza o instala ningun paquete. |
| `sudo apt upgrade` | Al actualizar la lista de repositorios y versiones, ejecutar upgrade se asegura de actualizar los paquetes instalados |
| `sudo pacman -Syuu` | Para actualizar los paquetes en Manjaro |
| `sudo pacman -S unrar zip unzip p7zip gzip bzip2` | Instalar paquetes para archivos comprimidos |

## Herramientas
### Procesos
|Comando|Descripcion|
| ------- | ------- |
| `ps -aux` | Muestra informacion sobre los procesos que estan corriendo en el sistema. Incluye la siguiente informacion USER, PID, %CPU, %MEM, VSZ, RSS, TTY, STAT, START, TIME, COMMAND |
| `pstree` | Imprime los procesos que estan corriendo en el sistema de forma de un arbol de procesos. |
| `top` | Muestra los procesos en tiempo real |
| `htop` | Igual que top para ver los procesos en tiempo real, pero no viene disponible en linux. Se debe instalar para ser utilizado  |


### Redes
|Comando|Descripcion|
| ------- | ------- |
| `ip addr` | Lista la direccion de red. Incluye informacion sobre la interfaz y protocolo. |
| `ping 127.0.0.1` | Se utiliza para verificar conexion al ip utilizado |

### Otros
|Comando|Descripcion|
| ------- | ------- |
| `uptime` | Nos indica el tiempo que ha estado corriendo el equipo. |
| `clear` | Limpia o borra el historial de la terminal |
| `cat archivo1.txt` | Imprime el contenido del archivo en el argumento |
| `cat listaDeBrowsers.txt | grep [expresion regular]` | Procesa linea por linea de un comando e imprimi la linea que cumple con el que cumple con la expresion regular. |
| `ps -aux | grep firefox` | Se utiliza para pasar el resultado de un comando a otro comando, permitiendo asi crear una cadena de comandos |
| `uname -a` | Informacion del kernel utilizado |
| `ls /bin > <archivo>` | Utilizado para imprimir o inyectar el resultado del comando en el destino o archivo |
| `history > <archivo>` | Imprime el historial de comandos al destino seleccionado |


## Manejo de Archivos y Directorios
Lista los archivos dentro del folder actual, acepta los parametros:

|Comando|Descripcion|
| ------- | ------- |
| `ls` | lista el contenido del directorio actual |
| `ls -al` | lista el contenido del directorio actual en forma de lista, incluyendo archivos ocultos |
| `ls -ld ./*` | lista solamentes los directorios en el directorio actual |
| `cd nombreDelFolder` | Se utiliza para navegar dentro de un directorio. |
| `pwd` | Imprimer la ruta del directorio actual |
| `touch archivo1.txt` | Es el comando utilizado para crear el archivo en posicion y nombre relativo al parametro. |
| `cp -rv <arhivo/directorio> <archivo/directorio>` | Copia de forma recursiva(-r) y verbosa(-v) el objeto indicado al destino |
| `mv -R <objeto> <destino>` | Mueve el objeto al destino seleccionado |


## Editor de texto
|Comando|Descripcion|
| ------- | ------- |
| `nano archivo1.txt` | Abre un editor de texto en terminal |
| `vi archivo1.txt` | Es un editor de texto un poco mas avanzado |


## Manejo de Usuarios

|Comando|Descripcion|
| ------- | ------- |
| `sudo useradd -m <nombre> -G wheel -p <password>` | Agregar un nuevo usuario en Manjaro |


## Manejo de Permisos
Asignar permisos a un archivo o fichero
- r: read (4)
- w: write (2)
- x: execute (1)

[+] implica agregar [-] implica remover
[a] all [u] user owner [g] group [o] others

|Comando|Descripcion|
| ------- | ------- |
| `chmod -R [dueno][grupo][otros] <archivo>` | Asignar permisos al archivo donde `dueno`, `grupo` y `otros` son numeros que representan el nivel de permiso asignado. |
| `chmod -R [t][simbolo][permisos] <archivo>` | t representa a quien va dirigido, simbolo es + o - para agregar o quitar un permiso, y permisos son las letras representando el permiso a asignar, se pueden asignar multiples por tipo separados por comas |

# Cron y Crontab
crontab -ecrontab -h


|Comando|Descripcion|
| ------- | ------- |
| `crontab -l` | Lista todos las tareas registradas por el usuario actual |
| `crontab -e` | Habilita la edicion del archivo crontab para editar o agregar tareas |


