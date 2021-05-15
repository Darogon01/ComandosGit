

<h1 align="center">:rocket::cut_of_meat:COMANDS GIT:cut_of_meat::rocket:</h1>
<p align="center"><img width="200rem" hight="auto" src="/Img/git.png"/></p>


---


- [Comandos básicos](#comandos-básicos)
- [Descripción y contexto](#descripción-y-contexto)


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

En resumidas cuentas nosotros realizamos cambios en nuestros archivos, el comando status verificará que archivos han sidos modificados. Cuando deseemos registrar esos cambios tendremos que agregarlos con ![git add <dir>/-A]así ya estará listo para poder hacer un commit. El commit realiza la copia de ese instante para poder volver en el tiempo si es que es necesario

    
