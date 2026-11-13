# Centro Médico Vida

## Descripción del proyecto

Página web estática que simula un sistema de reserva de horas médicas. Permite seleccionar una especialidad, fecha y horario de atención.

El servicio utiliza Nginx mediante Docker y no requiere base de datos.

## Requisitos

- Docker Desktop instalado y en ejecución.
- Docker Compose disponible.
- Navegador web.
- Puerto 8080 disponible.

## Ejecución del proyecto

1. Descargar o clonar el repositorio de GitHub.
2. Abrir PowerShell en la carpeta del proyecto.
3. Construir la imagen e iniciar el contenedor:

    `docker compose up -d --build`

4. Abrir el navegador e ingresar a:

    http://localhost:8080

## Verificación del servicio

Comprobar el estado del contenedor:

`docker compose ps`

Verificar la respuesta HTTP:

`curl.exe -I http://localhost:8080`

Revisar los registros:

`docker logs centro-medico-vida`

Consultar el consumo de recursos:

`docker stats --no-stream centro-medico-vida`

## Detener el servicio

Para detener y eliminar el contenedor:

`docker compose down`