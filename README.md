# apuntes-git

Todo sobre los comandos git: BASICO, INTERMEDIO y AVANZADO

## COMANDOS MAS UTILIZADOS

```bash
git log --oneline

# Git Rebase lo que hace es que al fusionar crea nuevos commits, es decir, afecta el cambio del historial.
# Usar rebase cuando queremos fusionar ramas features con otras ramas features, pero, usar merge, para fusionar ramas features con master o dev.
git rebase [branch]

# Crear y moverse a nueva rama.
git checkout -b <rama>

# Clonar repositorio con el último commit
git clone --depth 1 <url-repository>

# Deshacer el commit y regresar los cambios al area de preparación para volver a comitear
git reset --soft HEAD~1

git stash save "mensaje"
git stash list
git stash apply stash@{0}
git reset --hard <commit>
git reset --soft <commit>
git merge [branch]
git pull
git commit -m "mensaje"
git status
git checkout .
git add .
git remote -v
git remote set-url origin <url-repository>
```

## BASICO

[Comandos git nivel Basico](README-basico.md)

## INTERMEDIO

[Comandos git nivel Intermedio](README-intermedio.md)

## AVANZADO

[Comandos git nivel Avanzado](README-avanzado.md)
