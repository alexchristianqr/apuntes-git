## BASICO

```bash
# Configuración inicial:
git config --global user.name "Alex Christian"
git config --global user.email "alexchristianqr@gmail.com"
```

```bash
# Gestión de cambios:
git add <ruta_archivo> # Añade un archivo al área de preparación.
git add . # Añade todos los archivos modificados y eliminados al área de preparación.
git commit -m "<mensaje_del_commit>" # Guarda los cambios en el repositorio.
```

```bash
# Revisión de cambios:
git status # Muestra el estado actual del repositorio.
git diff # Muestra las diferencias entre los archivos que no han sido preparados.
```

```bash
# Sincronización de cambios:
git pull # Obtiene y fusiona los cambios desde un repositorio remoto.
git pull origin <nombre_rama> 
git push # Envía tus commits locales a un repositorio remoto.
git push origin <nombre_rama>
```

```bash
# Ramas (Branches):
git branch # Lista todas las ramas locales.
git branch <nombre_rama> # Crea una nueva rama.
git checkout <nombre_rama> # Cambia a la rama especificada.
git merge <nombre_rama> # Fusiona la rama especificada con la rama actual.
```

```bash
# Gestión de historial:
git log # Muestra el historial de commits.
git reset --hard <commit> # Resetea el HEAD actual al commit especificado.
```
