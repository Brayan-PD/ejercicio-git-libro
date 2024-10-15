# Para comenzar debes de realizar la clonación del repositorio https://github.com/tu-usuario/ejercicio-git-libro mediante la siguiente secuencia de comandos:
<div aling="justify"> 

```code
bae2@jpexposito-VirtualBox:~$ git clone https://github.com/Brayan-PD/ejercicio-git-libro
Clonando en 'ejercicio-git-libro'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Recibiendo objetos: 100% (3/3), listo.

bae2@jpexposito-VirtualBox:~$ cd ejercicio-git-libro/

bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ ls -la
total 16
drwxrwxr-x  3 bae2 bae2 4096 oct 10 18:00 .
drwxr-x--- 22 bae2 bae2 4096 oct 10 18:00 ..
drwxrwxr-x  8 bae2 bae2 4096 oct 10 18:01 .git
-rw-rw-r--  1 bae2 bae2  488 oct 10 18:03 README.md

```
## Ejercicio 1
### Crear la carpeta capítulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto.

```code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ mkdir capítulos
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ cd capítulos/

bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ touch capitulo1.txt

bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ nano capitulo1.txt 

Añadimos el texto:
Git es un sistema de control de versiones ideado por Linus Torvalds.
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git add .
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git commit -m "Añadido capítulo 1"
[main 791e2e0] Añadido capítulo 1
 1 file changed, 1 insertion(+)
 create mode 100644 "cap\303\255tulos/capitulo1.txt"
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git log
commit 791e2e01f59d91539ef16b7725a1a341aa316359 (HEAD -> main)
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Thu Oct 10 18:23:02 2024 +0100

    Añadido capítulo 1

commit 8a4d0b636317bc037cb816003acf6fcea31dd41f (origin/main, origin/HEAD)
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Thu Oct 10 17:59:30 2024 +0100

    Initial commit
```
## Ejercicio 2
### Crear el fichero capitulo2.txt en la carpeta capítulos con el siguiente texto.

```code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ touch capitulo2.txt 
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ nano capitulo2.txt
Se le añade el texto:
El flujo de trabajo básico con Git consiste en:
 1- Hacer cambios en el repositorio.
 2- Añadir los cambios a la zona de intercambio temporal.
 3- Hacer un commit de los cambios.
 bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git add .
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git commit -m "Añadido capítulo 2"
[main efe4404] Añadido capítulo 2
 1 file changed, 4 insertions(+)
 create mode 100644 "cap\303\255tulos/capitulo2.txt"
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git log
commit efe440484f844ee32a9b05d55cfefddabcc34f39 (HEAD -> main)
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Thu Oct 10 18:35:01 2024 +0100

    Añadido capítulo 2

commit 791e2e01f59d91539ef16b7725a1a341aa316359
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Thu Oct 10 18:23:02 2024 +0100
```
## Ejercicio 3
### Crear el fichero capitulo3.txt en la carpeta capítulos con el siguiente texto.
```code
Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.

    Añadir los cambios a la zona de intercambio temporal.
    Hacer un commit de los cambios con el mensaje Añadido capítulo 3.
    Mostrar las diferencias entre la primera y la última versión del repositorio.
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ ls
capítulos  README.md
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ cd capítulos/
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ touch capitulo3.txt 
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ nano capitulo3.txt 
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git log
commit 15f63b9fb88a0f06f04d9ee59ddede1db9b65d54 (HEAD -> main)
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Mon Oct 14 15:43:51 2024 +0100

    Añadido capítulo 3.

commit efe440484f844ee32a9b05d55cfefddabcc34f39
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Thu Oct 10 18:35:01 2024 +0100

    Añadido capítulo 2
commit 15f63b9fb88a0f06f04d9ee59ddede1db9b65d54 (HEAD -> main)
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Mon Oct 14 15:43:51 2024 +0100

    Añadido capítulo 3.

commit efe440484f844ee32a9b05d55cfefddabcc34f39
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Thu Oct 10 18:35:01 2024 +0100

    Añadido capítulo 2

commit 791e2e01f59d91539ef16b7725a1a341aa316359
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Thu Oct 10 18:23:02 2024 +0100

    Añadido capítulo 1

commit 8a4d0b636317bc037cb816003acf6fcea31dd41f (origin/main, origin/HEAD)
Author: brayan-pd <brayanpaezdiaz1@gmail.com>
Date:   Thu Oct 10 17:59:30 2024 +0100

    Initial commit

[1]+  Detenido                git log
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git diff efe440484f844ee32a9b
05d55cfefddabcc34f39..HEAD
diff --git "a/cap\303\255tulos/capitulo3.txt" "b/cap\303\255tulos/capitulo3.txt"
new file mode 100644
index 0000000..6e501ab
--- /dev/null
+++ "b/cap\303\255tulos/capitulo3.txt"
@@ -0,0 +1 @@
+Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.
```
## Ejercicio 4
### Crea el fichero índice.txt la siguiente línea:
```code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ touch indice.txt
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ nano indice.txt
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git add .
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git commit -m "Se crea el ind
ice."
[main bbcd5a6] Se crea el indice.
 1 file changed, 1 insertion(+)
 create mode 100644 "cap\303\255tulos/indice.txt"
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$  echo "Indice de los cápitulos, con conceptos avanzados de git" >> indice.txt
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git add .
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$  git commit -m "Añadido el índice ."
[main 502bef9] Añadido el índice .
 1 file changed, 1 insertion(+)
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$  git annotate indice.txt
bbcd5a6b        ( brayan-pd     2024-10-14 16:17:57 +0100       1)Indice de los cápitulos, con conceptos avanzados de git
502bef9a        ( brayan-pd     2024-10-14 16:18:24 +0100       2)Indice de los cápitulos, con conceptos avanzados de git
```
## Ejercicio 5
### Crear una nueva rama bibliografía y mostrar las ramas del repositorio.
```code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$   git branch bibliografia
  git branch -av
  bibliografia        502bef9 Añadido el índice .
* main                502bef9 [adelante 5] Añadido el índice .
```
## Ejercicio 6
### Crear el fichero capitulos/capitulo4.txt y añadir el texto siguiente:
```code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ touch capitulo4.txt
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ ls
capitulo1.txt  capitulo2.txt  capitulo3.txt  capitulo4.txt  indice.txt
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ nano capitulo4.txt 
  "En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto."
  
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git log --graph --all --oneline
* 7bfa7ac (HEAD -> bibliografia) se añade el capitulo4
* 0334bc0 (origin/main, origin/HEAD, main) Se hacen los ejecicios hasta el 4
* 502bef9 Añadido el índice .
* bbcd5a6 Se crea el indice.
* 15f63b9 Añadido capítulo 3.
* efe4404 Añadido capítulo 2
* 791e2e0 Añadido capítulo 1
* 8a4d0b6 Initial commit
```
## Ejercicio 7
### Cambiar a la rama bibliografía.Crear el fichero bibliografia.txt y añadir la siguiente referencia:

```code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ touch bibligrafia.txt
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ nano bibligrafia.txt 
Chacon, S. and Straub, B. Pro Git. Apress.
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git add .
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git commit -m "Añadida primera referencia bibliográfica."
[bibliografia ce9f16c] Añadida primera referencia bibliográfica.
 1 file changed, 1 insertion(+)
 create mode 100644 "cap\303\255tulos/bibligrafia.txt"
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro/capítulos$ git log --graph --all --oneline
* ce9f16c (HEAD -> bibliografia) Añadida primera referencia bibliográfica.
* 7bfa7ac se añade el capitulo4
* 0334bc0 (origin/main, origin/HEAD, main) Se hacen los ejecicios hasta el 4
* 502bef9 Añadido el índice .
* bbcd5a6 Se crea el indice.
* 15f63b9 Añadido capítulo 3.
* efe4404 Añadido capítulo 2
* 791e2e0 Añadido capítulo 1
* 8a4d0b6 Initial commit
```
## Ejercicio 8
### Fusionar la rama bibliografía con la rama main.
### Mostrar la historia del repositorio incluyendo todas las ramas.
### Eliminar la rama bibliografía.
### Mostrar de nuevo la historia del repositorio incluyendo todas las ramas.

```code
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ git branch 
  bibliografia
* main
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ git merge bibliografia 
Actualizando 0334bc0..ce9f16c
Fast-forward
 "cap\303\255tulos/bibligrafia.txt" | 1 +
 "cap\303\255tulos/capitulo4.txt"   | 1 +
 2 files changed, 2 insertions(+)
 create mode 100644 "cap\303\255tulos/bibligrafia.txt"
 create mode 100644 "cap\303\255tulos/capitulo4.txt"
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$  git log --graph --all --oneline
* ce9f16c (HEAD -> main, bibliografia) Añadida primera referencia bibliográfica.
* 7bfa7ac se añade el capitulo4
* 0334bc0 (origin/main, origin/HEAD) Se hacen los ejecicios hasta el 4
* 502bef9 Añadido el índice .
* bbcd5a6 Se crea el indice.
* 15f63b9 Añadido capítulo 3.
* efe4404 Añadido capítulo 2
* 791e2e0 Añadido capítulo 1
* 8a4d0b6 Initial commit
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ git branch -d bibliografia
Eliminada la rama bibliografia (era ce9f16c).
bae2@jpexposito-VirtualBox:~/ejercicio-git-libro$ git log --graph --all --oneline
* ce9f16c (HEAD -> main) Añadida primera referencia bibliográfica.
* 7bfa7ac se añade el capitulo4
* 0334bc0 (origin/main, origin/HEAD) Se hacen los ejecicios hasta el 4
* 502bef9 Añadido el índice .
* bbcd5a6 Se crea el indice.
* 15f63b9 Añadido capítulo 3.
* efe4404 Añadido capítulo 2
* 791e2e0 Añadido capítulo 1
* 8a4d0b6 Initial commit
```
# Ejercicio 9
### Crear la rama bibliografía.
### Cambiar a la rama bibliografía.
### Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias:

```code

```
</div>