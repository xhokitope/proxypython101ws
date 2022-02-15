# Proxy Python 101 WEBSOCKET

# INICIO:

apt-get update && apt-get upgrade -y

sudo su

cd

# Archivo para crear proxy python con conexion HTTP/1.1 101 para conexiones websocket.

# Puerto Default Dropbear 8080, puede editar el archivo con edotor de texto, Nano o Vim para modificar el puerto preferido para Dropbear.

DEFAULT_HOST = '127.0.0.1:8080'


# El Puerto proxy python tiene por default el 80, tambien puede editar a su preferencia.

LISTENING_PORT = 80

# Para activar el servicio proxy python websocket lanzar uno de los siguientes comando:

# Puede Usar TMUX:

tmux

python proxysocket.py 80

Salir con [CONTROL] + [b] + [d]

# O usar SCREEN

screen python proxysocket.py 80

Si no termina la ejecucion del comando en 10 segundos solo cerrar consola y volver a abrir.

# En cualquiera de los 2 casos la respuesta del comando seria:

:-------PythonProxy-------:

Listening addr: 0.0.0.0
Listening port: 80

:-------------------------:

# Si no hay ningun error ese seria el mensaje de respuesta.

# Revizar los puertos activos con el comando:

netstat -tnlp

# Antes de usar el servicio proxy python 101 debe tener instalado python

apt-get install python




# @XhokitoPe




