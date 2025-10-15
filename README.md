# LaboratorioSO_cliente_servidor
🧠 Cliente y servidor en C que se comunican por FIFO (Named Pipe). Laboratorio de Sistemas Operativos – Pontificia Universidad Javeriana.

Este laboratorio implementa dos programas en C (cliente y servidor) que se comunican entre sí mediante una FIFO (tubería con nombre) ubicada en /tmp/fifo_twoway.

El servidor crea la FIFO, recibe cadenas desde el cliente y devuelve la versión invertida del texto.

El cliente envía mensajes y muestra las respuestas del servidor.

Al enviar la palabra end, ambos procesos finalizan ordenadamente.


🧠 Explicación técnica

FIFO (Named Pipe): canal especial del sistema de archivos que permite comunicación bidireccional entre procesos.

open(): abre o crea el archivo FIFO con permisos 0640 (rw-r-----).

mkfifo(): crea la FIFO si no existe.

read() / write(): permiten el envío y recepción de cadenas.

sleep(2) en el servidor evita que lea su propio mensaje antes que el cliente.
