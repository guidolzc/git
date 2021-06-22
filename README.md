#GIT 
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

git rm historia.txt =  buscalo y ahora q hago con el lo tiene como en la nube ram

git rm --cached historia.txt  = borra ese txt  del git de subida pero no lo borra de la carperta +

git add historia.txt = lo agregamos de nuevo 

git commit -m " este es mi primer comit"


//////////////////////////////////////////////////////////////////////////////////////////////////////

# Configurar Git

Configuración del usuario

git config --global user.email "guidoit2021@gmail.com"

git config --global user.name "guido"


////////////////////////////////////////////////////////////////////////////////////////////////////////
# GIT agregando modificaciones 
cat historia.txt  = veo lo q es ta escrito 

code historia.txt = abre el archivo en visual studio code modifico la edad 31

git status = para ver en rojo q se a modificado 

vuelvo agregar 
git add .  == agrego lo q modifique

una vez modificado  adderido correctamente  podre modificar el commit 

$ git commit -m "este es mi primer commit de este archivo cambiando mi edad correcta"


git log historia.txt = ve el historia de q modificaste correo usuario horario y lo q modificaste 

///////////////////////////////////////////////////////////////////////////////////////////////////////

# como saber como se rompio un codigo 

verificamos donde estamos 

$ pwd

luego vemos lo q se encuentra adentro

$ ls 

modificamos lo que queremos modificar 

$code historia.txt

volvemos agregar la modificacion 

$ git add . 

agregamos el commit 

$ git commi    = aqui se abrira una ventana donde mostrara que agregemos un commit agregamos y listo

volvemos agregar la modificacion 

$ git add . 

vemos los cambios modificados  para ver los ultimos comandos que se han echo 

$ git show  


si queremos ver el historial 

$ git log historia.txt


luego de ejectur git log  historia.txt  aqui ponemos el commit de la historia primera y luego la historia modificada del commit con espacio en el medio de los 2 codigos
veremos claramente la modificaciones echas 

$ git diff  a3522d7cb8abbf739facd89e7e8fe5bad3f58227  d0bc310a3e4e616821cffaa9faa78de1d938380b


////////////////////////////////////////////////////////////////////////////////////////////////////





