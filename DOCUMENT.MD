# Creación de una página Web utlizando Herramientas de Git y GitHub

Creamos un nuevo repositorio en GitHub llamado DiarioAlia

![imagen](https://user-images.githubusercontent.com/71660964/96142818-ca1a3b00-0f02-11eb-8aca-ec2aa576c170.png)

Y una carpeta en mi ordenador donde guardaremos los archivos del proyecto 

![imagen](https://user-images.githubusercontent.com/71660964/96143118-182f3e80-0f03-11eb-9011-0a2aa6cb0c0b.png)

Creamos un archivo llamado index.html (mostramos archivo)

![imagen](https://user-images.githubusercontent.com/71660964/96143798-bfac7100-0f03-11eb-9cb7-500639c6f3e1.png)

ahora vamos a crear el primer commit, para ello tenemos que iniciar git,  hacerle seguimiento al archivo que queremos subir....

```sh
$ git init
$ git status
$ git add index.html
$ git commit -m "Esqueleto básico index.html"

```
### Aquí subimos a GitHub los commits que creamos
```sh
$ git remote add origin https://github.com/apaisgarcia/DiarioAlia.git
$ git push origin master
```
![imagen](https://user-images.githubusercontent.com/71660964/96145333-62192400-0f05-11eb-96ee-d6c1c2228e9d.png)

ahora vamos a subir otro commit con la cabecera

![imagen](https://user-images.githubusercontent.com/71660964/96146554-b40e7980-0f06-11eb-9677-9261a383a77f.png)

volvemos a realizar lo mismo que hicimos anteriormente

![imagen](https://user-images.githubusercontent.com/71660964/96146760-f0da7080-0f06-11eb-9e0d-ae44c350def2.png)
 Este sería el nuevo código del index.html

![imagen](https://user-images.githubusercontent.com/71660964/96147523-b2918100-0f07-11eb-8de9-b9ac506c8414.png)
Añadimos el nuevo archivo
![imagen](https://user-images.githubusercontent.com/71660964/96147951-1156fa80-0f08-11eb-8ee0-369abccff642.png)

Tambien se pueden subir todos los archivos a la rama utilizando este código

```sh
$ git push -o origin --all
$ git push -o origin --tags

```

Con esta instrucción vemos origin 

``` sh
$ git remote -v
```

![imagen](https://user-images.githubusercontent.com/71660964/96150599-d4403780-0f0a-11eb-80cb-1e5f5aca47d4.png)

Creamos varios artículos en el index.html

![imagen](https://user-images.githubusercontent.com/71660964/96150468-ae1a9780-0f0a-11eb-9947-e2c261549918.png)

ahora vamos a crear el commit , esta vez no lo subimos todavía al proyecto

![imagen](https://user-images.githubusercontent.com/71660964/96151024-444ebd80-0f0b-11eb-9356-34f2be1d7ee2.png)

Creamos una hoja de estilos.css llamada style.css

![imagen](https://user-images.githubusercontent.com/71660964/96151628-ed95b380-0f0b-11eb-8d26-a92ab81422bd.png)

y realizamos el seguimiento y un commit


``` sh
$ git add style.css
$ git commit -m "añadimos .css del html y body"
```
**_En alguna ocasión puedo utilizar_**
``` sh
$ git add .
```
**_Esto se utiliza cuando quiero subir varios archivos y así no los nombro uno por uno._**

![imagen](https://user-images.githubusercontent.com/71660964/96151839-29c91400-0f0c-11eb-849a-6f08036cca29.png)

Modificamos el archivo

![imagen](https://user-images.githubusercontent.com/71660964/96152851-487bda80-0f0d-11eb-845a-4a9936e9c135.png)

Creamos un commit con las nuevas modificaciones

![imagen](https://user-images.githubusercontent.com/71660964/96153098-92fd5700-0f0d-11eb-96aa-8624285a67c8.png)

Ponemos el logo en la barra izquierda, para ello creamos una carpeta llamada images
![imagen](https://user-images.githubusercontent.com/71660964/96241737-dfdf3d00-0fa2-11eb-8dde-c55186b7ab52.png)
![imagen](https://user-images.githubusercontent.com/71660964/96241877-0e5d1800-0fa3-11eb-8f34-168094082de5.png)

Añadimos el commit al proyecto -> 

![imagen](https://user-images.githubusercontent.com/71660964/96241990-3b112f80-0fa3-11eb-9b10-c45f19eb55ac.png)

Modificamos el css añadiendo datos al section
![imagen](https://user-images.githubusercontent.com/71660964/96242454-c38fd000-0fa3-11eb-9d59-ba6e4ba36ab7.png)

Y añadimos el commit

![imagen](https://user-images.githubusercontent.com/71660964/96242578-e621e900-0fa3-11eb-8771-21d69fe71b76.png)

Añadimos al css la parte del pie de página 

![imagen](https://user-images.githubusercontent.com/71660964/96242780-2719fd80-0fa4-11eb-9227-8eb93515aa8d.png)

Y añadimos un commit indicado los nuevos cambios

```sh
$ git add style.css
$ git commit -m " añadimos footer al css"
```

![imagen](https://user-images.githubusercontent.com/71660964/96242931-5af52300-0fa4-11eb-8950-b2f7f42537a9.png)

Realizamos cambios en el css 

![imagen](https://user-images.githubusercontent.com/71660964/96243403-fedece80-0fa4-11eb-81c4-771abbc272d9.png)

Hacemos un commit indicándolo

![imagen](https://user-images.githubusercontent.com/71660964/96243635-4c5b3b80-0fa5-11eb-8398-6eda884c933b.png)

**_Observamos que al utilizar git add . -> tambien añadimos la carpeta de imagenes_**

Actulalizamos en GitHub con todos nuestros cambios 

```sh
$ git push origin master

```
![imagen](https://user-images.githubusercontent.com/71660964/96243849-96dcb800-0fa5-11eb-873b-9748d86b2f7a.png)

###Vemos los cambios en GitHub

![imagen](https://user-images.githubusercontent.com/71660964/96244492-6a756b80-0fa6-11eb-98f1-8d06f9a80857.png)

![imagen](https://user-images.githubusercontent.com/71660964/96244408-52055100-0fa6-11eb-93eb-673285a5cff7.png)

_**Etiquetas -> Se utilizan para marcar puntos específicos del historial como importantes**_

```sh
$ git tag -a v1.0 -m "Versión 1.0"
```
![imagen](https://user-images.githubusercontent.com/71660964/96245531-b543b300-0fa7-11eb-96cc-4db09c96ac34.png)

Para ver si tengo etiquetas y enseñar se puede utilizar 
```sh
$ git tag 
```
```sh
$ git show v1.0
```
![imagen](https://user-images.githubusercontent.com/71660964/96246051-621e3000-0fa8-11eb-8a6b-a97d41333d79.png)

Creamos una rama y nos posicionamos en ella

```sh
$ git branch develop
$ git checkout develop
```

![imagen](https://user-images.githubusercontent.com/71660964/96246354-cccf6b80-0fa8-11eb-8618-1efdb3dd023a.png)

Creamos una carpeta llamada imagenes

```sh
$ mkdir imagenes

```
y metemos la foto del logo.png y realizamos un commit 

![imagen](https://user-images.githubusercontent.com/71660964/96247019-cb527300-0fa9-11eb-87a3-a3e16eaaf753.png)

Creamos un directorio llamado CSS y movemos a esa carpeta el archivo style.css

```sh
$ mkdir css
$ mv style.css css
```
![imagen](https://user-images.githubusercontent.com/71660964/96247395-5cc1e500-0faa-11eb-8980-bff9f3980a5e.png)

Hacemos un git status para observar como está la carpeta

```sh
$ git status

```

![imagen](https://user-images.githubusercontent.com/71660964/96247581-9a267280-0faa-11eb-9e83-e88bd1c4fc59.png)

Realizamos un commit con los nuevos cambios

![imagen](https://user-images.githubusercontent.com/71660964/96247784-e07bd180-0faa-11eb-9fc6-124a110b5a5e.png)

Añadimos un commit con la nueva organización , ya que cambiamos en el index.html para que salga la foto que está guardada en la actualidad en la carpeta imagenes.

![imagen](https://user-images.githubusercontent.com/71660964/96248317-abbc4a00-0fab-11eb-9fbf-d70e518e4d22.png)

ahora vamos a Actualizar la página, para subir todos nuestros cambios

![imagen](https://user-images.githubusercontent.com/71660964/96248649-2a18ec00-0fac-11eb-8343-00e25d1c587c.png)

ahora vamos a confirmar los cambios en GitHub


![imagen](https://user-images.githubusercontent.com/71660964/96248795-677d7980-0fac-11eb-8bba-8338a6c1d6f9.png)

![imagen](https://user-images.githubusercontent.com/71660964/96249067-e7a3df00-0fac-11eb-8614-ae21905ac3b9.png)

Desde GitHub confirmo el Pull request y le doy autorización a la fusión de datos 


![imagen](https://user-images.githubusercontent.com/71660964/96249854-1f5f5680-0fae-11eb-9061-355cc6a47a53.png)

y vemos todo el código unificado 

![imagen](https://user-images.githubusercontent.com/71660964/96249973-55043f80-0fae-11eb-92b0-c624c744bc67.png)

# Ahora desde github.com

creamos una rama desde el entorno gŕafico de GitHub

![imagen](https://user-images.githubusercontent.com/71660964/96284010-4da85a80-0fdd-11eb-8e65-865f9be3d391.png)

Hago una modificación en el archivo style.css  (elimino los comentarios de  bordes)

![imagen](https://user-images.githubusercontent.com/71660964/96284557-04a4d600-0fde-11eb-8b0c-e643171b64f6.png)

![imagen](https://user-images.githubusercontent.com/71660964/96284260-9fe97b80-0fdd-11eb-9f30-e6a8f257489e.png)

![imagen](https://user-images.githubusercontent.com/71660964/96284522-f8b91400-0fdd-11eb-824f-260f4c4b9bb9.png)
Hago un cambio en el index.html , Pongo como título "Diari Alia"
![imagen](https://user-images.githubusercontent.com/71660964/96284747-5188ac80-0fde-11eb-89a2-201e5d0010cb.png)
y creo el commit
![imagen](https://user-images.githubusercontent.com/71660964/96284893-83017800-0fde-11eb-8ee0-452b5c5d4bcf.png)

elimino la C (del copyrigth ) y cambio el año 2012 por 2018

![imagen](https://user-images.githubusercontent.com/71660964/96285521-5d28a300-0fdf-11eb-9175-4041fe5b5876.png)

Creo una tag

Creamos una etiqueta con la versión 1.1

![imagen](https://user-images.githubusercontent.com/71660964/96287022-96faa900-0fe1-11eb-96ad-ba3ea1abb294.png)

![imagen](https://user-images.githubusercontent.com/71660964/96287261-f5278c00-0fe1-11eb-96bc-2a6d955568bb.png)

![imagen](https://user-images.githubusercontent.com/71660964/96287349-16887800-0fe2-11eb-9bf7-aa312929bc9e.png)

y lo confirmo 

![imagen](https://user-images.githubusercontent.com/71660964/96287402-2acc7500-0fe2-11eb-81b2-426075476b12.png)
Queda así GitHub

![imagen](https://user-images.githubusercontent.com/71660964/96287462-45065300-0fe2-11eb-8f42-c14b57c442fa.png)

Borramos la rama bugfix desde GitHub

![imagen](https://user-images.githubusercontent.com/71660964/96334102-80e6fa00-106e-11eb-9f46-57359573eb28.png)

Queda de esta manera..

![imagen](https://user-images.githubusercontent.com/71660964/96334123-9c520500-106e-11eb-8505-057d541291ae.png)

_Observamos que deja la opción de restaurarla, si quisieramos hacerlo en algún momento_

Creamos una etiqueta v1.2

![imagen](https://user-images.githubusercontent.com/71660964/96334178-fd79d880-106e-11eb-8c02-dda9a0a15779.png)

Vemos como queda

![imagen](https://user-images.githubusercontent.com/71660964/96334190-1d110100-106f-11eb-90c6-c8924fc139c6.png)

Creamos un nuevo fichero llamado DOCUMENT.MD (con toda la tarea realizada hasta ahora)

![imagen](https://user-images.githubusercontent.com/71660964/96334324-25b60700-1070-11eb-8d28-ac7e157ef3e9.png)

![imagen](https://user-images.githubusercontent.com/71660964/96334271-c35d0680-106f-11eb-9f8c-37e87150bb27.png)

![imagen](https://user-images.githubusercontent.com/71660964/96334310-0b7c2900-1070-11eb-897d-5ffc891c062b.png)

Queda el proyecto de esta manera 

![imagen](https://user-images.githubusercontent.com/71660964/96334340-4c743d80-1070-11eb-8547-be91031972a6.png)

Ahora vamos a crear una  **gh-page** 

**_Esto crea una rama de código especial llamada gh-pages que es publicada en una ubicación especial_**

![imagen](https://user-images.githubusercontent.com/71660964/96335111-48e3b500-1076-11eb-9dc0-283b5cd09880.png)

Vemos como queda la rama y el respositorio

![imagen](https://user-images.githubusercontent.com/71660964/96335220-77ae5b00-1077-11eb-8132-7670141a7a84.png)

```sh
  https://apaisgarcia.github.io/DiarioAlia/
```
Creamos en master el archivo README.md

![imagen](https://user-images.githubusercontent.com/71660964/96335439-de804400-1078-11eb-8229-bcd55f7b8c01.png)

![imagen](https://user-images.githubusercontent.com/71660964/96335600-1cca3300-107a-11eb-9bd3-bfbfddfb14eb.png)


**Como podemos ver el enlace ?**

![imagen](https://user-images.githubusercontent.com/71660964/96335636-64e95580-107a-11eb-83c0-f6eb188d5a0f.png)

![imagen](https://user-images.githubusercontent.com/71660964/96335659-77638f00-107a-11eb-9801-bdfb56ec9a29.png)

Y así queda el enlace si lo abres :

![imagen](https://user-images.githubusercontent.com/71660964/96335749-08d30100-107b-11eb-8292-a81b14c1045d.png)

```sh
**Anotación: En algunos ordenadores deja el logo a la izquierda y la escritura a la derecha.
```

## Repositorio Local

Ahora vamos a actualizar la carpeta que tenemos en nuestro escritorio (repositorio remoto)


![imagen](https://user-images.githubusercontent.com/71660964/96336299-0ecae100-107f-11eb-985f-3b42798531b8.png)

Vemos lo que tenemos en la carpeta (los archivos)

![imagen](https://user-images.githubusercontent.com/71660964/96336319-27d39200-107f-11eb-9b5c-2ea342cb402c.png)

Y para ver que todo esté bien miramos el archivo README.md (podríamos revisar todo, pero el este archivo es pequeño y para lo que queremos ver es suficiente)

![imagen](https://user-images.githubusercontent.com/71660964/96336335-48035100-107f-11eb-8bc0-da505af6e83f.png)

## Generando conflictos

Ahora vamos a realizar cambios para tener conflictos

creamos una nueva rama y realizamos cambios sobre el color de la página

![imagen](https://user-images.githubusercontent.com/71660964/96489041-2c46a900-123f-11eb-8692-6e4693b25d5a.png)

![imagen](https://user-images.githubusercontent.com/71660964/96489141-526c4900-123f-11eb-8de6-9dc09bacbb61.png)

ahora volvemos a master y realizamos un cambio en el css , le pongo que quiero el fondo rojo.
![imagen](https://user-images.githubusercontent.com/71660964/96489433-bbec5780-123f-11eb-9696-90955f918719.png)

![imagen](https://user-images.githubusercontent.com/71660964/96489296-8e9fa980-123f-11eb-9848-be6d192352ae.png)



Arreglamos el conflicto

![imagen](https://user-images.githubusercontent.com/71660964/96490885-be4fb100-1241-11eb-8b57-8052fbf1b624.png)

Y vemos como queda desde GitHub

![imagen](https://user-images.githubusercontent.com/71660964/96491344-649bb680-1242-11eb-8d77-f5566782f60b.png)

