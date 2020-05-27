# Sistemas Operativos(C2020-162013G2) - ULACIT

## Tabla de Contenidos
- [Bitacora de comandos](#lista-de-comandos)

## Lista de Comandos

### Comando especiales
- `sudo` es un prefijo que se asegura de ejecutar el comando con privilegios de administrador o "root".
- `apt` es el administrador de paquetes avanzado que viene disponible en muchas distribuciones de linux.

#### UPDATE
Actualiza los paquetes disponibles y sus versiones, pero no actualiza o instala ningun paquete.
```bash
$ sudo apt update
```

#### UPTIME
Nos indica el tiempo que ha estado corriendo el equipo
```bash
$ uptime
```

#### UPGRADE
Al actualizar la lista de repositorios y versiones, ejecutar upgrade se asegura de actualizar los paquetes instalados
```bash
$ sudo apt upgrade
```

#### IP ADDR
Lista la direccion de red. Incluye informacion sobre la interfaz y protocolo.
```bash
$ ip addr
```

#### PING
Se utiliza para verificar conexion al ip utilizado
```bash
$ ping 127.0.0.1
```

#### CLEAR
Limpia o borra el historial de la terminal
```bash
$ clear
```

#### LS
Lista los archivos dentro del folder actual, acepta los parametros:
- `-l` lista
- `-a` todos incluye los archivos y folderes ocultos
```bash
$ ls
$ ls -la
$ ls -l -a
```

#### CD
Se utiliza para navegar dentro de un directorio.
```bash
$ cd nombreDelFolder
$ cd nombreDelFolder/subfolder

$ cd /nombreDelDirectorio
# Una / al inicio de la ruta se utiliza como alias al "root" o directorio raiz principal.

$ cd ../../nombreDelFolder
# Los .. son utilizados para retroceder uno o mas niveles al utilizar ../../

$ cd
# Solo utilizar cd nos lleva al home del usuario en terminal
```

#### PWD
Imprimer la ruta del directorio actual
```bash
$ pwd
# ~ es un alias especial a la carpeta inicio del usuario
```

#### TOUCH
Es el comando utilizado para crear el archivo en posicion y nombre relativo al parametro.
```bash
$ touch archivo1.txt
```

#### NANO
Abre un editor de texto en terminal
```bash
$ nano archivo1.txt
```

#### CAT
Imprime el contenido del archivo en el argumento
```bash
$ cat archivo1.txt
```

#### VI
Es un editor de texto un poco mas avanzado
```bash
$ vi archivo1.txt
```

#### PS
Muestra informacion sobre los procesos que estan corriendo en el sistema. Incluye la siguiente informacion USER, PID, %CPU, %MEM, VSZ, RSS, TTY, STAT, START, TIME, COMMAND
```bash
$ ps -aux
```

#### GREP
Procesa linea por linea de un comando e imprimi la linea que cumple con el que cumple con la expresion regular.
```bash
$ cat listaDeBrowsers.txt | grep [expresion regular]
```

#### OPERADOR PIPE
Se utiliza para pasar el resultado de un comando a otro comando, permitiendo asi crear una cadena de comandos
```bash
$ ps -aux | grep firefox
```

#### PSTREE
Imprime los procesos que estan corriendo en el sistema de forma de un arbol de procesos.
```bash
$ pstree
```

#### TOP
Muestra los procesos en tiempo real
```bash
$ top
```

#### HTOP
Igual que top para ver los procesos en tiempo real, pero no viene disponible en linux. Se debe instalar para ser utilizado
```bash
$ htop
```


