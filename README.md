# Practica 5- SPRINGBOOT

Durante esta quinta práctica se procede a desarrollar una API REST con SpringBoot. Para ello inicialmente se accede al link https://start.spring.io/ para generar el proyecto.

Se ha reutilizado la práctica anterior para realizar un formulario de registro implementando un endpoint implementado con SpringBoot.

Para ello, se ha añadido una séptima página html denominada **registrarse.html**  a la cual se puede acceder pinchando en FanStore. La idea es realizar un formulario de registro de usuario, en el que se introducen los datos personales junto con una contraseña.  Como este apartado se ha hecho en SpringBoot se ha de levantar su servidor para que en la dirección http://localhost:8080/ aparezca la siguiente ventana:

![image](https://user-images.githubusercontent.com/98181428/159173673-3daa3e5a-b793-453a-9ce2-69f926b3616f.png)



- El formulario que he usado para implementar Spring-Boot ha sido el de registro del usuario. En http://localhost:8080/ se le pide nombre, apellidos, edad, identificación y contraseña. Se comprueba cuando el usuario da al submit que ninguno sea null, que la edad sea > 18 y que todos los campos menos la edad tengan de 2 a 30 caracteres. Si todo es correcto, se le redirige a result.html (http://localhost:8080/info) y le muestra el JSON creado con la información. En cambio, si hay algun error de los mencionados, muestra la misma página (regisrarse.html) para que el usuario corrija los errores junto a los mensajes de error correspondientes. 
- He hecho uso Thymeleaf: https://www.thymeleaf.org/ en registrarse.html.
- He usado Java Bean Validation’s @Valid constraint para validar los campos introducidos.
- Si algo ha ido mal en el funcionamiento de esta práctica, salta a la pagina error.html mostrando un mensaje.
