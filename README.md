Repositorio campusciff
===================

En este documento se recoge la siguiente información para los ejercicios de git:

- Comandos
- Explicaciones
- Capturas de pantalla

### 2.1.1 Crear repositorio remoto llamado campusciff
```
curl -u 'marcoscortina' https://api.github.com/user/repos -d '{"name":"campusciff"}'
```

### 2.1.2 Clonar repositorio en github
```
git clone https://github.com/marcoscortina/campusciff
```

### 2.2.1 Crear README.md y subirlo al repositorio remoto
```
touch README.md
```

### 2.3.1 Commit inicial
```
git commit -a -m "commit inicial"
```
![](https://github.com/marcoscortina/campusciff/raw/master/img/CommitInicial.png)


### 2.3.2 Subir los cambios al repositorio remoto
```
git push origin master
```

### 2.4.1 Crear archivo privado.txt
```
touch privado.txt
```

### v 2.4.2 Crear carpeta “privada” 
```
mkdir privada
```

### 2.4.3 Crear archivo .gitignore e insertar 2 líneas, una para ignorar el archivo privado.txt y otra para ignorar la carpeta privada
```
touch .gitignore
echo "privado.txt" >> .gitignore
echo "privada" >> .gitignore
```

### 2.5.1 Crear fichero
```
touch 1.txt		
```

### 2.5.2 Crear tag
```
git tag -a v0.1 -m 'versión 0.1'
```

### 2.5.3 Subir los cambios al repositorio remoto
```
git commit -a -m "Nuevos ficheros y creación de tag"
git push origin master
```		
					
###  2.6.1 Crear rama v0.2 y posicionarse en ella
```
git branch v0.2
```

### 2.6.2 Posicionarse en la rama v0.2 
```
git checkout v0.2
```

### 2.6.3 Crear archivo 2.txt
```
touch 2.txt
```

### 2.6.4 Subir los cambios al repositorio remoto
```
git commit -a -m "Creación de rama v0.2 y de archivo 2.txt"
git push origin v0.2
```


### 2.7.1 Posicionarse en la rama master
```
git checkout master
```


###  2.7.2 Hacer un merge de la rama v0.2 en la rama master
```
git merge v0.2
```

### 2.8.1 En la rama master poner Hola en el fichero 1.txt y hacer commit
```
git checkout master
echo "Hola" >> 1.txt
git add . 
git commit -m "Añadido Hola al fichero 1.txt"
```

### 2.8.2 Posicionarse en la rama v0.2 y poner Adiós en el fichero 1.txt y hacer commit
```
git checkout v0.2
echo "Adiós" >> 1.txt
git add .
git commit -m "Añadido Adiós al fichero 1.txt"
```

### 2.8.3 Posicionarse en la rama master y hacer el merge con v0.2
```
git checkout master
git merge v0.2
```

### 2.8.4 Listar ramas con merged y sin merge
```
git branch --no-merged 
git branch --merged
```

### 2.8.5 Arreglar conflicto
```
echo "Hola y adios" >> 1.txt
git add .
git commit -m "Corregido conflicto"
```
### 2.9.1 Crear un tag v0.2
```
git checkout v0.2
git tag v0.2
git checkout master
```

### 2.9.2 Listar los distintos commits con sus ramas y sus tags
```
git log --graph --pretty="%h %d %s"
```

### 2.9.3 Borrar la rama v0.2
```
git branch -d v0.2
```

### 2.10 Foto, autentificación y clave pública 

![](https://github.com/marcoscortina/campusciff/raw/master/img/FotoDePerfil.png)

![](https://github.com/marcoscortina/campusciff/raw/master/img/DobleFactorDeAutentificacion.png)

![](https://github.com/marcoscortina/campusciff/raw/master/img/ClavePublica.png)

###2.11.1 Uso social de GitHub. Seguir a mis compañeros.

![](https://github.com/marcoscortina/campusciff/raw/master/img/UsoSocialGitFollowing.png)

###2.11.1 Uso social de GitHub. Seguir repositorios y marcarlos con una estrella

![](https://github.com/marcoscortina/campusciff/raw/master/img/UsoSocialGitHubStars.png)



### 2.12 Crear una tabla

| Nombre     					| Usuario de GitHub 
| :-------------------------- 	| -------------------------- 
|Adolfo Sanz De Diego			|https://github.com/asanzdiego
|Alfonso Peña					|https://github.com/alfonsops
|Borja Moreno Pozo				|https://github.com/bmpozo
|Carlos Saiz Alves				|https://github.com/Carsaiz
|Francisco Javier Rivas Torres	|https://github.com/jrivax
|Juan José Díaz López			|https://github.com/jjdiazl
|Juan Ramón Márquez				|https://github.com/marquezjr
|Rodrigo Marcos Carvajal		|https://github.com/romcra



### 2.13 Poner a github.com/asanzdiego como colaborador del repositorio campusciff


### 2.14 Crear una organización llamada campusciff-marcoscortina
ok

### 2.15

Crear 2 equipos en la organización campusciff-marcoscortina, uno llamado administradores con más permisos y otro colaboradores con menos permisos.


#Meter a github.com/asanzdiego y a 2 de vuestros compañeeros de clase en el equipo administradores.

### 2.15.3 Meter a github.com/asanzdiego y a otros 2 de vuestros compañeros de clase en el equipo colaboradores.

https://github.com/marcoscortina

### 2.16.1 Crear un index.html que se pueda ver como página web en la organización.

ttp://campusciff-marcoscortina.github.io/marcoscortina.github.io

### 2.17

Hacer 2 forks de 2 repositorios campusciff- tunombredeusuariodegithub.github.io de 2 organizaciones de las que no seais ni administradiores ni colaboradores.

Crearos una rama en cada fork.

En cada rama modificar el fichero index.html añaadiendo vuestro nombre.

Con cada rama hacer un pull-request.

https://github.com/marcoscortina

### 2.18.1 Aceptar los pull-request que lleguen a los repositorios de tu organización.

https://github.com/marcoscortina






