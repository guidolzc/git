# GIT 
git init ,
git remote add origin LINK,
git status,
git add *    o git add .   ,
git status
git commit -m " name ",
git push origin master ,




 git add . === es para modificar lo q hayas echo un cambio a la version 1 
git cat vacio.txt  = para ver todo lo q esta escrito 
git history   = todos los comando q hicieron y si quiero usar el comando pongo el numero de comando 

rm historia.txt = en consola borra todo 

control + L O E borra todo lo q escribiste 

`git rm historia.txt` =  buscalo y ahora q hago con el lo tiene como en la nube ram

`git rm --cached historia.txt ` = borra ese txt  del git de subida pero no lo borra de la carperta +

`git add historia.txt` = lo agregamos de nuevo 

`git commit -m " este es mi primer comit"`


//////////////////////////////////////////////////////////////////////////////////////////////////////

# Configurar Git

Configuración del usuario
`git config`
`git confing --list  para ver la lista para modificar `

para ver donde esta las cosas guardadas casos avanzados 
`git config --list --show-origin   `

`git config --global user.email "guidoit2021@gmail.com"`

`git config --global user.name "guido"`

 para ver la lista para modificar  
`git confing --list   `        

////////////////////////////////////////////////////////////////////////////////////////////////////////
# GIT agregando modificaciones 
`cat historia.txt`  = veo lo q es ta escrito 

`code historia.txt `= abre el archivo en visual studio code modifico la edad 31

`git status `= para ver en rojo q se a modificado 

vuelvo agregar 
`git add .`  == agrego lo q modifique

una vez modificado  adderido correctamente  podre modificar el commit 

`$ git commit -m "este es mi primer commit de este archivo cambiando mi edad correcta"`


`git log historia.txt `= ve el historia de q modificaste correo usuario horario y lo q modificaste 

///////////////////////////////////////////////////////////////////////////////////////////////////////

# como saber como se rompio un codigo 

verificamos donde estamos 

`$ pwd`

luego vemos lo q se encuentra adentro

`$ ls `

modificamos lo que queremos modificar 

`$code historia.txt`

volvemos agregar la modificacion 

`$ git add . `

agregamos el commit siempre agregar "" un mensaje y quien somos nosotros "

`$ git commi  `  = aqui se abrira una ventana donde mostrara que agregemos un commit agregamos y listo

volvemos agregar la modificacion 

$ git add . 

# HISTORIAL Y COMPARACIONES
vemos los cambios modificados  para ver los ultimos comandos que se han echo 
`$ git show historia.txt`
commit 49061c8be016cae9ac7ee97d60f3165573cae3fe (HEAD -> master)  quiere decir q estoy en la version mas reciente


si queremos ver el historial 

`$ git log historia.txt`


luego de ejectur git log  historia.txt  aqui ponemos el commit de la historia primera y luego la historia modificada del commit con espacio en el medio de los 2 codigos
veremos claramente la modificaciones echas 

aqui comparamos los 2 commit
`$ git diff  a3522d7cb8abbf739facd89e7e8fe5bad3f58227  d0bc310a3e4e616821cffaa9faa78de1d938380b`


////////////////////////////////////////////////////////////////////////////////////////////////////
# RAMAS
staging es la memoria ram es el estado temporal al q agregamos archivos que vamos cambiando y el repositorio real es cuando nosotrodamos commit 

tracked es cuando ve la historia 

commit -m  ya hacemos el cambio q hacemos en el repositorio y cada comit es v1 . v2. v3 .v4 etc.

checkout traerte una version anterior  o un cambio anterior o la ultima version

//////////////////////////////////////////////////////////////////////////////////////////

# MARGE
marge  = es cuando tengo varias Versiones v1 , v 2 . v 3. v 4  si la v4 es el actual version y tiene bug hacemos un una copia y cuando modificamos y lo volvemos armar otra version nueva modificando sacando el bugfixig=hotpix resolver los cambios ya mismos eso se llamara un marge ....

 unes la v2 experimentada a la proyecto final tambien se considera un marge 
        
puede salir tambien experimentos de otra version y asi van uniendo al proyecto final o pueden experimentar el proyecto final y luego unir las versiones experimentadas

al unir otro experimento de bugfixins crea otra version final final

bugfixig=hotpix
hotpix == son lo q tienen q salir YA MISMO

/////////////////////////////////////////////////////////////////////////////////////////////
# RESET

HARD

para volver un tiempo atras usamos  el codigo que queremos volver y lo demas que hicimos borrara todo 

`$git reset a3522d7cb8abbf739facd89e7e8fe5bad3f58227 --hard `        

----------------------------------------------------------------------------
SOFT

aqui sigue  los elementos en STAGING de trabajo por ejemplo lo que agregaste con ADD .

`$git reset a3522d7cb8abbf739facd89e7e8fe5bad3f58227 --soft  `        

----------------------------------------------------------------------------


////////////////////////////////////////////////////////////////////////////////////////////////////////////////
# CREAR Y VER NUEVOS CAMBIOS 

cuando creamos algo nuevo  PODEMOS VER LAS MODIFICACIONES con git STATUS Y LUEGO git DIFF

`$ git diff` ==  muestra el directorio actual osea en mi disco y en mi  STAGING 


`$ git log --stat ` ==  para ver la cantidad de numeros de cambios 

-----------------------------------------------------------------------------------
aqui volvemos en el tiempo a cierta carpeta  podemos saltar de un cambio a otro ....... OBVIO SIN DAR COMMIT hasta estar seguros....

`$ git checkout a3522d7cb8abbf739facd89e7e8fe5bad3f58227 historia.txt `

`$ git commit -am `= guarda cambios solo funciona si ya habias guardado con add previamente


# CREA RAMAS  moviendose por HEAD

`$ git branch cabecera`   ===== CREA LA RAMA Y LA MUESTRA

`$git show `    mostrara las ramas MASTER , CABEZERA o donde estoy PARADO

`$git checkout CABEZERA   `   <---- ponemos el nombre de la rama "CABEZERA y cambiamos de RAMA 

`$git add . `

`$git commit -m "cambios editados en master "`

`$git checkout master`	<---- veo los ultimos commit o add


`$git checkout CABEZERA`   <---- veo los ultimos commit o add

`$git add .`

`$git commit -m "cambios editados en cabezera "`



# EDITANDO MASTER Y CABEZERA cada uno con su distinto commit y luego uniendolos 

`$ git checkout master `

funcionamos la CABEZERA al MASTER
`$ git merge cabecera `


FUCION 
`$ git branch` ==== le indica donde estas o q ramas estas

`$ git checkout master `

funcionamos la CABEZERA al MASTER
`$ git merge cabecera `

`$ git log      `     y vemos  master los commit y los commit de cabezera 

`$git add .    `         == modificamos la fusion la letras 

`$git commit - m  "volvi a una tipografia ARIAL"`

`$ git log  `               == para ver los cambios


CONFLICTO 2 PERSONAS CAMBIARON EL MISMO CODIGO hablar con la persona y elegir q codigo tomar y guardar 



# REMOTO ya trabajando en un repositorio creado

1 `$ pwd   ` ====== Reviso que estoy en mi carpeta 

2 `$ git remote add origin https://github.com/guidolzc/pro2.git`Aqui ponemos el NOMBRE ORIGIN Y LA PAGINA QUE AREMOS EL REMOTO 

3 `$ git remote -v   `

origin  https://github.com/guidolzc/pro2.git (fetch)  === traer cosas

origin  https://github.com/guidolzc/pro2.git (push)  ==== enviar cosas

4 ` $ git pull origin main --allow-unrelated-histories `   ==== traeme todos los datos del github a mi repositorio local


5 `$ ls`  === MIRAMOS O fijamos q nos trae README.md  

 si tienes el correo igual que el github no te pedira contraseña
 
6 `$ git push origin master:main`    === SUBE mi repositorio  ONLINE al MAIN pero cuidado modifico todo o puedo eliminar algo que no actualize para volver a subir

7 `$ git pull origin main `     ==  TRAE los datos cambiados o puestos por otra persona de GITHUB a mi repositorio LOCAL
  `From github.com:guidolzc/pro2* branch            main       -> FETCH_HEAD  Already up to date `

8 * ` $git branch -m main ` -m mueve todo los cambios exitentes en tu rama MASTER  a la nueva rama MAIN

9 `$ git push origin main`  al hacer esto ahora ya funcionaria para enviar al REMOTO

# trabajando por SSH

1 `ssh-keygen -t rsa -b 4096 -C "pcigfernandez@gmail.com"`  ponemos nuestro correo local para crear la llave

2 `$ eval $(ssh-agent -s)`   vericar q el servidor esta corriendo o q el proceso esta encendido

3  `~ ` este signo nos indica donde ir a seleccionar para mostrar en mi pc 

4 ` $ cd ~/.ssh/   `   == entramos a la carpeta .ssh y seleccionamos la llave

5 `$ ssh-add ~/.ssh/id_rsa`     == elegimos la pass pribada nunca compartir   = las llaves publica y pribada las 2 son 1 por pc

6 Nos dirigimos a nuestro perfil de Github `github / configuracion / ssh and gpg keys / SSH key `y colocamos aqui la key PUBLICA 

7 git remote -v 

8 $ git remote set-url origin git@github.com:guidolzc/pro2.git

9 git remote -v

10 `$  git pull` YES para que verifique la keys y union con mi pc para que ya no deje entrar a otro q no sea yo 

11  `$ git pull origin main` para probar si estamos actualizados  antes de hacer un commit 

12 `$git status `    para ver el CAMBIO que puse al HTML v2.02021

13 `$ git diff`     para ver que cambie y que escribi

14 `$ git commit -am "v 2.2021"`    recien guardo lo que cambie 

15 `$ git pull origin main`   hacemos el pull para actualizarnos

16 `$ git push origin main`    para enviar los datos cambiados en el servidor LOCAL al REMOTO

# COMANDOS  TAGS
`$ git log --all --graph --decorate --oneline`  es para mostrar una forma resumida los branch los commit las ramas


`$ alias arbolito="git log --all --graph --decorate --oneline"`de esta forma pongo mis TAGS mas cortos referidos a 1 ALIAS 


`$ arbolito` aqui me mostrara todo igual q TAG que es muy largo para escribit y asi creamos nuestros porpios ALIAS TAGS


