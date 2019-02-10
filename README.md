# [PHP_] - APILoginRegister

## Español

Éste pequeño ejercicio consiste en una pequeña API Rest realizada con PHP Nativo (Eso significa el PHP_ en el titulo) que será de utilidad para algunos usuarios que deseen implementar un login (inicio de sesión) y un registro para usuarios, así como su control en una base de datos, funciona a través de peticiones __HTTP__.

Fue realizado bajo la siguiente arquitectura:

* Servidor Apache (Wampserver 3.1.3)
* PHP Versión 7.0.29
* MySQL versión 5.7.21

### Pasos previos

* Deberás crear una base de datos llamada __login_api__ con un cotejamiento __utf8_general_ci__, ir a la sección SQL e importar el archivo __login_api.sql__ que se sitúa en la carpeta __query__

### Cosas a considerar

* La API se comunica a través del protocolo __HTTP__ y en específico peticiones __POST__ para enviar los parámetros sin que estos viajen por la URL si no en la cabecera.
* Los parámetros que recibe al hacer la petición en la URL **_../../register_** son:
    * __name__
    * __email__
    * __password__
* Los parámetros que recibe al hacer la petición en la URL **_../../login_** son:
    * __email__
    * __password__
* Las respuestas __positivas__ de las peticiones son en formato __JSON__ con los siguientes paráametros:
    * __uuid__
    * __name__
    * __email__
    * __created_at__
    * __updated_at__
    * __login_status__
* Las respuestas __negativas__ de las peticiones son en formato __JSON__ con los siguientes parámetros:
    * __error__
    * __error_msg__

## English

This small exercise consists of a small API Rest made with PHP Native (That means the PHP_ in the title) that will be useful for some users who wish to implement a login and a registry for users, as well as its control in a database, It works through requests __HTTP__.

It was made under the following architecture:

* Apache Server (Wampserver 3.1.3)
* PHP Version 7.0.29
* MySQL versión 5.7.21

### Previous steps

* You must create a database called __login_api__ with a collation __utf8_general_ci__, go to the SQL section and import the file __login_api.sql__ that is placed in the folder __query__

### Things to know

* The API communicates through the __HTTP__ protocol and in specific __POST__ requests to send the parameters without them traveling through the URL if not in the header.
* The parameters that you receive when making the request in the URL **_/login/register_** are:
    * __name__
    * __email__
    * __password__
* The parameters that you receive when making the request in the URL **_/login/login_** are:
    * __email__
    * __password__
* The __positive__ responses of the requests are in __JSON__ format with the following parameters:
    * __uuid__
    * __name__
    * __email__
    * __created_at__
    * __updated_at__
    * __login_status__
* The __negative__ responses of the request are in __JSON__ format with the followuing parameters:
    * __error__
    * __error_msg__