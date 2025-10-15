# LaboratorioSO_cliente_servidor
🧠 Cliente y servidor en C que se comunican por FIFO (Named Pipe). Laboratorio de Sistemas Operativos – Pontificia Universidad Javeriana.

Este laboratorio implementa dos programas en C (cliente y servidor) que se comunican entre sí mediante una FIFO (tubería con nombre) ubicada en /tmp/fifo_twoway.

El servidor crea la FIFO, recibe cadenas desde el cliente y devuelve la versión invertida del texto.

El cliente envía mensajes y muestra las respuestas del servidor.

Al enviar la palabra end, ambos procesos finalizan ordenadamente.
