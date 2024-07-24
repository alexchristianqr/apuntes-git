# apuntes-git

Todo sobre los comandos git: BASICO, INTERMEDIO y AVANZADO

## BASICO

[Comandos git nivel Básico](README.md)

## INTERMEDIO

[Comandos git nivel Intermedio](README-intermedio.md)

## AVANZADO

```bash
# Deshacer cambios:
git reset --soft <commit> # Restablece solo el puntero de la rama actual (HEAD), dejando el índice y el directorio de trabajo sin cambios. Los cambios confirmados anteriormente pero no empujados al repositorio remoto quedarán en el índice, listos para ser confirmados nuevamente si es necesario. Referencia <commit>: HEAD, HEAD~1, branch_name, commit
git reset --soft HEAD~1 # Último commit en la rama
git reset --soft HEAD~2 # Penultimo commit en la rama
git reset --soft HEAD~3 # Antepenultimo commit en la rama
git reset --hard <commit> # Restablece tanto el índice como el directorio de trabajo. Los archivos modificados pero no confirmados serán descartados. Referencia <commit>: HEAD, HEAD~1, branch_name, commit
```

```bash
# Cleaning (limpieza de archivos no deseados):
git clean -f # Elimina archivos no rastreados.
git clean -fd # Elimina directorios no rastreados.
```

```bash
# Worktree (múltiples directorios de trabajo):
git worktree add <directorio> <rama> # Añade un nuevo directorio de trabajo vinculado a una rama.
git worktree list # Lista todos los directorios de trabajo.
```

```bash
# Blame (seguimiento de cambios en líneas específicas):
git blame <archivo> # Muestra quién cambió cada línea de un archivo y en qué commit.
```

```bash
# Rebase avanzado:
git rebase --onto <nuevo_base> <rama_base> <rama> # Rebase la rama especificada sobre una nueva base.
git rebase -i HEAD~<n> # Rebase interactivo para los últimos n commits.
```

```bash
# Reflog (registro de referencias):
git reflog # Muestra un historial de todos los cambios en los punteros (HEAD, ramas, etc.).
git reset --hard <reflog-entry> # Restaura el repositorio a un estado anterior utilizando una entrada de reflog.
```

```bash
# Submódulos (Submodules):
git submodule add <repositorio> <ruta> # Añade un submódulo.
git submodule update --init --recursive # Inicializa, clona y actualiza todos los submódulos.
git submodule deinit <ruta> # Desinicializa un submódulo.
```

```bash
# Manipulación de ramas remotas:
git remote prune origin # Elimina referencias a ramas remotas que ya no existen en el servidor.
git push origin <rama>:<nueva_rama> # Empuja una rama local a una rama remota con un nombre diferente.
```

```bash
# Bisect (búsqueda binaria de errores):
git bisect start # Inicia una búsqueda binaria para encontrar el commit que introdujo un bug.
git bisect good <commit> # Marca un commit como bueno.
git bisect bad <commit> # Marca un commit como malo.
git bisect reset # Termina la búsqueda binaria y vuelve al estado original.
```