# apuntes-git

Todo sobre los comandos git: BASICO, INTERMEDIO y AVANZADO

## BASICO

[Comandos git nivel Básico](https://github.com/alexchristianqr/apuntes-git/blob/main/README.md)

## INTERMEDIO

```bash
# Deshacer cambios:
git reset <archivo> # Quita el archivo del área de preparación.
git checkout -- <archivo> # Deshace los cambios en un archivo no preparado.
```

```bash
# Manipulación de commits:
git commit --amend # Modifica el último commit (útil para cambiar el mensaje del commit o agregar archivos omitidos).
git revert <commit> # Crea un nuevo commit que revierte los cambios de un commit anterior.
```

```bash
# Rebase:
git rebase <rama_base> # Reaplica los commits de la rama actual sobre la rama base especificada.
git rebase -i <commit> # Rebase interactivo para editar, combinar o reordenar commits.
```

```bash
# Stash (guardar cambios temporalmente):
git stash # Guarda los cambios sin commit temporalmente.
git stash pop # Aplica los cambios guardados con git stash y los elimina de la lista de stash.
git stash list # Muestra la lista de cambios guardados en el stash.
git stash apply stash@{0}
git stash save "<mensaje>"
```

```bash
# Cherry-pick (aplicar un commit específico a otra rama):
git cherry-pick <commit> # Aplica los cambios de un commit específico en la rama actual.
```

```bash
# Buscar en el historial:
git log --grep="<mensaje>" # Busca commits cuyo mensaje contenga la palabra especificada.
git log -p # Muestra las diferencias introducidas en cada commit.
```

```bash
# Alias (crear atajos para comandos):
git config --global alias.co checkout # Crea un alias para el comando git checkout.
```

```bash
# Cambiar la URL de un repositorio remoto:
git remote set-url origin <url_github_repositorio> # Cambia la URL del repositorio remoto.
```

## AVANZADO

[Comandos git nivel Avanzado](https://github.com/alexchristianqr/apuntes-git/blob/main/README-avanzado.md)