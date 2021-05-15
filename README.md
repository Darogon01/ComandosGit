

<h1 align="center">:rocket::cut_of_meat:COMANDS GIT:cut_of_meat::rocket:</h1>
<p align="center"><img width="200rem" hight="auto" src="/Img/git.png"/></p>


---


- [Comandos básicos](#comandos-básicos)
- [Ramas o branch](#ramas-o-branch)
- [Crear una nuevo repositorio](#Crear-una-nuevo-repositorio)
- [Push](#push)
- [Pull](#pull)
- [Fetch](#fetch)
- [Clonar repositorio](#lonar-repositorio)


---

<p align="center"><img width="450rem" hight="auto" src="/Img/git-flujo.png"/></p>

Explicando la imagen: Tenemos nuestro directorio local (una carpeta en nuestro pc) con muchos archivos, Git nos irá registrando los cambios de archivos o códigos cuando nosotros le indiquemos, así podremos viajar en el tiempo retrocediendo cambios o restaurando versiones de código, ya sea en Local o de forma Remota (servidor externo). En la práctica quedará más claro.

---

### Comandos básicos

Conocer la versión de git instalada.
```javascript
git version
```

Ayuda sobre los comandos.
```javascript
git help
```

Iniciar un nuevo repositorio.
```javascript
git init
```

// Ver que archivos no han sido registrados.
```javascript

git status
```
Agregar todos los archivos los al staging área.<img width="200rem" hight="auto" src="/Img/add-file SD.png"/>
```javascript
git add -A
```

Agrega el archivo que elijamos al staging área.
```javascript
git add <dir> 
```

Crear commit (fotografía del proyecto en ese momento).
```javascript
git commit -m "primer commit"
```

// Muestra la lista de commit del mas reciente al más antigüo.
```javascript
git log
```

En resumidas cuentas nosotros realizamos cambios en nuestros archivos, el comando ```git status``` verificará que archivos han sidos modificados. Cuando deseemos registrar esos cambios tendremos que agregarlos con ```git add dir/-A``` así ya estará listo para poder hacer un ```git commit -m ""```. El commit realiza la copia de ese instante para poder volver en el tiempo si es que es necesario. A continuación estaremos listos para subirlo a nuestro repositorio remoto con ```git push```.

---

### Ramas o branch.


Crea una nueva rama.
```javascript
git branch <nombre-de-rama>
```

Nos muestra en que rama estamos.
```javascript
git branch
```

Para ver las ramas que tiene el repositorio en remoto.
```javascript
git branch -A
```

Nos movemos a la nueva rama.
```javascript
git checkout <nombre-de-rama>
```

Nos movemos a la nueva rama.
```javascript
git checkout <nombre-de-rama>
```
Podemos unir la rama main con la nueva, para eso tenemos que estar en la main para ejecutar el siguiente comando:

Fusiona la rama que indiquemos en el comando con la rama en la que estamos actualmente.
```javascript
git merge <nombre-de-rama>
``` 
Para crear una rama nueva y movernos a ella en un solo comando.

```javascript
git checkout -b <nombre-de-rama>
``` 

Eliminar una rama.
```javascript
git branch -d <nombre-de-rama>
``` 
---
### Crear una nuevo repositorio

Para subir nuestro proyecto debemos crear un nuevo repositorio, al momento de la creación nos mostrará una serie de comandos para subir el proyecto.
```javascript
git remote add origin https://github.com/bluuweb/tutorial-github.git
git push -u origin master
``` 

Nos muestra en que repositorio estamos enlazados remotamente.
```javascript
git remote -v
```
---
### Push

```javascript
git remote -v
```

Al ejecutar el comando `git push` estaremos subiendo todos los cambios locales al servidor remoto de github, ten en cuenta que tienes que estar enlazado con tu repositorio, para eso puedes utilizar `git remote -v` y luego ejecuta:
```javascript
git push
```
---
### Pull

Cuando realizamos cambios directamente en github pero no de forma local, es esencial realizar un pull, donde descargaremos los cambios realizados para seguir trabajando normalmente.
Es importante estar enlazados remotamente, puedes verificar con: `git remote -v`, luego ejecuta:
```javascript
git pull
```
---
### Fetch

Este comando hace la comparación de nuestros archivos locales con los del servidor, si existiera alguna diferencia nos pediría realizar un `get pull` para realizar un match de nuestros arhivos locales.

```javascript
git fetch
```
