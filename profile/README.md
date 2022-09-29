
<h1 align="center"> Pet's care</h1>
<p align="center"> El proyecto PET 'S CARE es un aplicativo WEB, el cual llega como una nueva alternativa para facilitar el proceso de un agendamiento de citas para las mascotas, a la que los dueños de mascotas puedan interactuar en una interfaz amigable con el objetivo de solicitar el servicio desde su casa, y los dueños de las mascotas puedan agendar una cita con la veterinaria de su preferencia.</p>

<p align="center"><img src="https://user-images.githubusercontent.com/86493588/193126183-371d741d-04ef-44aa-a6e9-0de57a059afc.jpeg" width="800"/></p> 

## Tabla de contenidos:

- [Stack de desarrollo](#stack-de-desarrollo)
- [Descripción y contexto](#descripción-y-contexto)
- [Guías de Uso por Roles](#guía-de-usuario)
- [Guía de instalación](#guía-de-instalación)
- [Autor/es](#autores)

## Stack de desarrollo

Para desarrollar el back-end, el front-end y el despliegue de este aplicatvo se utilizaron las siguientes tecnologias.

### Back-end : 
para realizar el back-end de este aplicativo se decidio utilizar el lenguage de programacion java, para realizar un api rest y utilizamos springboot para facilitar el mapeo de entidades, tambien se utilizo swager para documentar la api, spring security para darle seguridad a los datos.
- [![Java](https://img.shields.io/badge/Java-FF0000?style=for-the-badge&logo=java&logoColor=white&labelColor=2E2C22)]()
[![MySQL](https://img.shields.io/badge/MySQL-93FF00?style=for-the-badge&logo=mysql&logoColor=white&labelColor=2E2C22)]()
[![spring boot](https://img.shields.io/badge/SpringBoot-2C971D?style=for-the-badge&logo=springboot&logoColor=1BE300&labelColor=2E2C22)]()

### Front-end
para el front-end se utilizaros las tres tecnologias bases de la web javascript, html y css y react para el renderizando de la componetes en una sola pagina. 
- [![JavaScript](https://img.shields.io/badge/JavaScript-informational?style=for-the-badge&logo=javascript&logoColor=FFF700&labelColor=2E2C22)]()
[![HTML](https://img.shields.io/badge/HTML5-FF8300?style=for-the-badge&logo=html5&logoColor=orange&labelColor=2E2C22)]()
[![css](https://img.shields.io/badge/CSS3-blue?style=for-the-badge&logo=css3&logoColor=blue&labelColor=2E2C22)]()
[![react](https://img.shields.io/badge/react-B5B5B5?style=for-the-badge&logo=react&logoColor=00F3FF&labelColor=2E2C22)]()
### Despliegue
para reaizar el despliegue de el back-end y la base de datos de este aplicativo se utilizo google cloud alludado por app-engine y cloud-sql y para deplegar el front-end se utilizo cloudflare.
- [![Google Cloud](https://img.shields.io/badge/googlecloud-yellow?style=for-the-badge&logo=googlecloud&logoColor=&labelColor=2E2C22)]()
[![Cloudflare](https://img.shields.io/badge/cloudflare-orange?style=for-the-badge&logo=cloudflare&logoColor=white&labelColor=2E2C22)]()

## Descripción y contexto
---
El objetivo para este proyecto es minimizar el tiempo de espera, y una mayor efectividad a la hora de agendar una cita, desde la comodidad de un teléfono inteligente o un computador de escritorio.

Tal como al se menciona al inicio, el proyecto PET 'S CARE es un aplicativo WEB ,el cual llega como una nueva alternativa para facilitar el proceso de un agendamiento de citas para las mascotas, a la  que los dueños de mascotas puedan interactuar en una interfaz amigable con el objetivo de solicitar el servicio desde su casa, y los dueños de las mascotas puedan agendar una cita con la veterinaria de su preferencia. La investigación en campo, se realiza en veterinarias del municipio del quindío, con el objetivo de conocer si cuentan con algún aplicativo web para  la atención de sus clientes y a su vez, conocer si cuentan con el servicio de agendamiento de citas online,adicionalmente, se realiza varias investigaciones sobre proyectos en donde se desarrollen aplicaciones web con actividades similares a la de solicitud de citas virtuales.

## Guías de Uso por Roles
---
Este aplicativo consta de 4 Roles (Administrador, Clinica, Veterinario, Usuario), para saber cual es el uso adecuado segun Rol consulte el manual respectivamente.

Como Usuario: <a href="https://github.com/PetsCare12/DocumentacionPetsCare/blob/main/Manual%20de%20usuario/PT-MU-01-Manual-cliente.docx">Consultar Manual de Usuario</a><br/>
Como Clinica: <a href="https://github.com/PetsCare12/DocumentacionPetsCare/blob/main/Manual%20de%20usuario/PT-MU-02-Manual-clinica.docx">Consultar Manual de Clinica</a><br/>
Como Veterinario: <a href="https://github.com/PetsCare12/DocumentacionPetsCare/blob/main/Manual%20de%20usuario/PT-MU-01-Manualdeusuario-Veterinario.docx">Consultar Manual de Veterinario</a><br/>
Como Administrador: <a href="https://github.com/PetsCare12/DocumentacionPetsCare/blob/main/Manual%20de%20usuario/PT-MU-02-Manual-administrador.docx">Consultar Manual de Administrador</a><br/>


## Guía de instalación

Para poder utilizar esta aplicacion de forma local debemos cumplir con unos requisitos previos que se espesifican a continuacion.

### Requisitos del sistema
- 4 GB de RAM
- 300 MB de espacio libre en disco duro
- Procesador Intel Core i3 o AMD Ryzen 3

### Herramientas de desarrollo

_Herramientas para desarrollo back-end_

* [Eclipse IDE](https://www.eclipse.org/downloads/) - Entorno de desarrollo integrado.
* [Spring Tool Suite]() - Entorno para trabajar spring.
* [JDK Java](https://www.java.com/es/) - Java DevKit.
* [Workbench]() - Administración de bases de datos
* [Xampp]() - Servidor local.

_Herramientas para desarrollo front-end_

* [VS code]() - Entorno de desarrollo integrado para react.</br>
* [NodeJS]() - Entorno de ejecucion.

_Paso a paso para ejecutar la aplicacion en local_

1. Clonar el repositorio del back-end y del front-end
2. Abrir la carpeta del back en springtoolsuite y la carpeta del front en vs code
3. Abrir xampp e iniciar el servidor apache y mysql
4. Abrir workbench y crear una bd con la siguiente sentencia;
``` 
create database petsCare1;
use petsCare1;
```
5. En springtool suite debe ir a el paquete de resource y en la clase properties debe cambiar lo siguiente
```
spring.datasource.url=jdbc:mysql://localhost:3306/petsCare1?useUnicode=true&useJDBCCompliantTimezoneShift=true&useLegacyDatetimeCode=false&serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password= 
```
- Añadir el localhost correspondiente
- Si su usuario es distinto a root tambien debera cambiarlo
- Y si su workbench tiene contraseña debera ponerlo alli 
cuando allamos realizado el paso anterior debera ejecutar el backend
6. Una vez echo el pazo anterio en mysql workbench ejecutaremos la siguiente sentencia

```
insert into roles (id, nombre_rol) 
values 
(1 , "ROLE_ADMIN"),
(2 , "ROLE_USER"),
(3 , "ROLE_CLINICA"),
(4 , "ROLE_VETERINARIO");

insert into usuarios (documento_usu,apellido_usu,correo_usu,estado_usu,foto_usu,nombre_usu,password_usu,sexo_usu,telefono_usu) values ('111', 'admin ', 'admin@gmail.com', '1', 'https://fotografias.lasexta.com/clipping/cmsimages02/2022/03/11/DD3ADEF0-EBDC-41D1-BE29-7FD5950B9005/anonymous_98.jpg?crop=4320,2431,x0,y136&width=1900&height=1069&optimize=high&format=webply', 'admin', 'admin', 'otro', 'admin'
);
insert into usuario_roles (usuario_doc,rol_id) values (1,1);
```
7. En la consola de vs code debe utilizar la siguiente sentencia para instalar los paquetes necesarios
```
npm install
```
Una vez alla terminado el proceso utilize el siguiente comando 
```
npm start
```


## Autor/es
---
* <a href="https://github.com/SamuelRm5">Samuel Rodriguez</a> - Desarrollador FrontEnd - DBA
* <a href="https://github.com/JuanVera326">Juan Vera</a> - Desarrollador FrontEnd - DevOps
* <a href="https://github.com/juaanmarin">Juan Marin</a> - Desarrollador BackEnd - DevOps
* <a href="https://github.com/kevynpinedasena">Kevyn Pineda</a> - Desarrollador BackEnd - DBA
* <a href="https://github.com/andres518">Andres Alvarez</a> - Desarrollador FrontEnd - Documentacion - Tester

