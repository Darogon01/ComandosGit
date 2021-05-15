

<h1 align="center">:rocket::cut_of_meat:COMANDS GIT:cut_of_meat::rocket:</h1>
<p align="center"><img width="200rem" hight="auto" src="/Img/git.png"/></p>


---


- [Comandos básicos](#comandos-básicos)
- [Ramas o branch](#ramas-o-branch)

---

<p align="center"><img width="400rem" hight="auto" src="/Img/git-flujo.png"/></p>

Explicando la imagen: Tenemos nuestro directorio local (una carpeta en nuestro pc) con muchos archivos, Git nos irá registrando los cambios de archivos o códigos cuando nosotros le indiquemos, así podremos viajar en el tiempo retrocediendo cambios o restaurando versiones de código, ya sea en Local o de forma Remota (servidor externo). En la práctica quedará más claro.

---

### Comandos básicos

```javascript
// Conocer la versión de git instalada
git version
```
```javascript
// Ayuda sobre los comandos
git help
```
```javascript
// Iniciar un nuevo repositorio
// Crear la carpeta oculta .git
git init
```
```javascript
// Ver que archivos no han sido registrados
git status
```
```javascript
// Agregar todos los al staging área.
git add -A
//Agrega el archivo que elijamos al staging área
git add <dir> 
```
```javascript
// Crear commit (fotografía del proyecto en ese momento)
git commit -m "primer commit"
```
```javascript
// Muestra la lista de commit del mas reciente al más antigüo
git log
```

En resumidas cuentas nosotros realizamos cambios en nuestros archivos, el comando ```git status``` verificará que archivos han sidos modificados. Cuando deseemos registrar esos cambios tendremos que agregarlos con ```git add dir/-A``` así ya estará listo para poder hacer un ```git commit -m ""```. El commit realiza la copia de ese instante para poder volver en el tiempo si es que es necesario. A continuación estaremos listos para subirlo a nuestro repositorio remoto con ```git push```.

### Ramas o branch

```javascript
// Crea una nueva rama
git branch <nombre-de-rama>
```
```javascript
// Nos muestra en que rama estamos
git branch
```
```javascript
//Para ver las ramas que tiene el repositorio en remoto
git branch -A
```
```javascript
// Nos movemos a la nueva rama
git checkout <nombre-de-rama>
```
```javascript
// Nos movemos a la nueva rama
git checkout <nombre-de-rama>
```
Podemos unir la rama main con la nueva, para eso tenemos que estar en la main para ejecutar el siguiente comando:

```javascript
// Fusiona la rama que indiquemos en el comando con la rama en la que estamos actualmente.
git merge <nombre-de-rama>
``` 

```javascript
// Para crear una rama nueva y movernos a ella en un solo comando
git checkout -b <nombre-de-rama>
``` 
```javascript
// Eliminar una rama
git branch -d <nombre-de-rama>
``` 

