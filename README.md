

<h1 align="center">:rocket::cut_of_meat:COMANDS GIT:cut_of_meat::rocket:</h1>
<p align="center"><img width="200rem" hight="auto" src="/Img/git.png"/></p>


---


- [Comandos básicos](#comandos-básicos)
- [Ramas o branch](#ramas-o-branch)


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
git branch nombreRama
```
```javascript
// Nos muestra en que rama estamos
git branch
```
```javascript
// Nos movemos a la nueva rama
git checkout nombreRama
```
Podemos unir la rama main con la nueva, para eso tenemos que estar en la main para ejecutar el siguiente comando:

```javascript
// Nos movemos a la nueva rama
git merge nombreRama
``` 
```javascript
// Eliminar una rama
git branch -d nombreRama
``` 

