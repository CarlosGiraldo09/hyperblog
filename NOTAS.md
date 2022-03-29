Git sirve para poder monitorear los cambios que se generan en un codigo de programación, tanto los que realice yo en solitario, como otro miembro de un grupo si trabajo en equipo.

De igual modo git sirve para generar diferentes ramas donde pueda realizar cambios sin afectar a la rama principal y poder implementarlos en un futuro o revertirlos de ser necesario.

Comandos:
git init → Iniciar directorio de trabajo

git add nombre → Agregar a git lo del nombre

git  commit -m “nombre” → guarda el cambio con un nombre

git add . → Agregar todo

git status → Saber los cambios

git -m “cambios” → 

git log → Muestra los Hash (código del commit creado) 

git show → Muestra el contenido de un archivo

git push → Para enviar a repositorio remoto

git pull → Trae todo al directorio actual

git checkout → Cambia de rama

git branch → Crea una rama

git diff → Compara commits

git commit -m “cambio” → Agrega automáticamente nombre al commit

git reset → Volvemos a una versión anterior

rm → Eliminar

rm -ri → Eliminar archivos completos con confirmación

git clone url → Cambia mi Directorio local por el directorio remoto

git fetch → Trae al repositorio local

git merge → Combina ramas

git config → Para saber mi configuración de git bash en local

Esc shift ZZ → cierra interfaz de agregar nombre de un commit

git remote add origin → creó un repositorio remoto

git remote -v → muestra que el repositorio ya está cargado

git push origin main → lleva mi repositorio local al remoto

hlc =git log --all --graph --decorate --oneline → historial de commits con dibujitos jeje

git rebase = es como un merge pero sin dejar evidencia en las historias

Si realizo un cambio desde el repositorio remoto en github es importante que lo traiga al local con el comando git pull origin main.

Para enviar al repositorio remoto los cambios cuando los hago en el repositorio local debo hacerlo con git push origin main para que se guarden.

Las llaves públicas y privadas son un par matemático para codificar y decodificar un mensaje secreto.

Para crear un pull request primero debo realizar un fork, después clonar el repositorio remoto al local con un git clone, después debo entrar a la carpeta donde esté el archivo desde la terminal y hacer git pull para traer los archivos, allí hago los cambios, hago un push para enviar a github. Entró al repositorio remoto original y hago la solicitud de pull request, comparó el original con mi fork y listo! a esperar.

Si quiero que un archivo binario u otro tipo de archivo no se cargue a github debo crear un .gitignore.

Cuando realizo un rebase primero lo hago de la rama que quiero eliminar y después de la rama main.

Un git stash me permite recuperar los cambios me permite poner en pausa un cambio al que no se le ha realizado un commit.
Despues con git stash pop vuelvo a hacer visible el cambio y lo puedo solucionar.
Si uso un stash hacia una rama crea esa branch y realiza los cambios alli. con git stash branch nombre de la branch.
Tambien puedo hacer un git stash drop para efectuar el cambio.

Git clean --dry-run me muesta los archivos que se van a eliminar al aplicar un git clean.

Git clean -f me limpia archivos a los cuales no les he hecho commit y que git lee como un error.

git cherry-pick con el hash integra un commit unico de una rama alterna a la main.