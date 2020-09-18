# backup
Script para respaldar bases de datos mongodb y rotar los respaldos viejos.

Instalacion
clon de git https://github.com/fulvous/backup.git

Uso
Uso: mongobackup [-f directorio_respaldo] [-d bases] [-o anterior_a] [-v]

Este script respalda bases de datos mongodb y rota sus dueños respaldos.

-f define el directorio en donde se respaldarán los datos.

-d Bases de datos a respaldar separadas por comas.

-o Se borraran los respaldos mas viejos a este numero de dias.

-v Muestra informacion adicional

Ejemplo de configuración en / etc / crontab:

0 2 * * * root / ruta_completa / mongobackup -f / opt / respaldos -d mi_base -o 2

Estora ejecuta el comando todos los dias a las 2am

Utilizara / opt / respaldos como el directorio de respaldos

Respaldara la base mi_base y la comprimira en 7z

Borrara los respaldos mayores a 2 dias

mongobackup
Script para hacer una copia de seguridad de la base de datos mongo y rotarla

