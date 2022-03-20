# Practica 5- SPRINGBOOT

Durante esta quinta práctica se procede a desarrollar una API REST con SpringBoot. Para ello inicialmente se accede al link https://start.spring.io/ para generar el proyecto.

Se ha reutilizado la práctica anterior para realizar un formulario de registro implementando un endpoint implementado con SpringBoot.

Para ello, se ha añadido una séptima página html denominada **registrarse.html**  a la cual se puede acceder pinchando en FanStore si se ejecutara la práctica como html. 

La idea es realizar un formulario de registro de usuario, en el que se introducen los datos personales junto con una contraseña. Como este apartado se ha hecho en SpringBoot se ha de levantar su servidor para que en la dirección http://localhost:8080/ aparezca la ventana de registrase.html que se muestra a continuación:

![Captura de pantalla 2022-03-20 a las 17 59 41](https://user-images.githubusercontent.com/98181428/159173714-02b4bb9c-054c-4f54-a6ab-a6c996a0953d.png)

Además el formulario hace una serie de comprobaciones y si algún campo está vacío lanza un mensaje de error, mostrando la misma página registrarse.html para que se corrija.

Además registrarse.html hace uso de 
- Thymeleaf: https://www.thymeleaf.org/ 
- Java Bean Validation’s @Valid constraint para validar los campos introducidos.

Una vez se rellena correctamente los datos del formulario aparece el json donde se han guardado los datos. A continuación se muestra cómo debería verse:


![Captura de pantalla 2022-03-20 a las 18 07 00](https://user-images.githubusercontent.com/98181428/159174091-b67e5d31-7048-4b28-bb54-2a08ef7a4791.png)

Decir que si se trata de accecer a las diferentes páginas html del menú que se muestra en registrase.html, va a mostrar un mensaje de error como el que se muestra a continuación:

![Captura de pantalla 2022-03-20 a las 18 03 36](https://user-images.githubusercontent.com/98181428/159173978-b74b5012-76b5-4a21-8a5e-8effad996646.png)

Dicho mensaje se encuentra en error.html y también se muestra si algo no funciona durante la práctica.


