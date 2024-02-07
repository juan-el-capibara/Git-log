# Git-log
1. En la terminal, ejecuta el comando git log --graph --decorate --oneline -n 5. Este comando mostrará un resumen gráfico de los últimos 5 commits en todas las ramas.
2. En la terminal, ejecuta el siguiente comando:
git log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all

Este comando mostrará un resumen gráfico del historial de commits con las siguientes especificaciones:

Una representación gráfica del historial de commits.
El hash corto del commit en color azul.
Las referencias (ramas o tags) en las que está involucrado el commit en color amarillo.
El mensaje del commit.
La fecha relativa del commit en color verde.
El hash del commit como un identificador abreviado.
Las fechas de los commits de forma relativa.
3. En la terminal, ejecuta el siguiente comando:
git config --global alias.last 'log -1 HEAD'

Este comando creará un alias llamado last que representará el comando git log -1 HEAD. Ahora puedes usar git last para ver el último commit.

Es importante mencionar que los alias de Git se almacenan en tu archivo de configuración de Git. Si deseas ver todos tus alias y configuraciones de Git, puedes usar el comando git config --list.

4. En la terminal, ejecuta el siguiente comando:
git config --global alias.ec 'config --global -e'

Este comando creará un alias llamado ec que abrirá la configuración global de Git en tu editor de texto preferido. Ahora puedes usar git ec para abrir la configuración global de Git

5 .En la terminal, ejecuta el siguiente comando:
git log --graph --abbrev-commit --decorate --format=format:'%C(red)%h%C(reset) - %C(yellow)%d%C(reset) %s %C(green)(%cr)%C(reset)' --all

Este comando mostrará un resumen gráfico del historial de commits con las siguientes especificaciones:

Una representación gráfica del historial de commits.
El hash corto del commit en color rojo.
Las referencias (ramas o tags) en las que está involucrado el commit en color amarillo.
El mensaje del commit.
La fecha relativa del commit en color verde.
