# [PHP_] - APILoginRegister

## Español

Éste pequeño ejercicio consiste en una pequeña API Rest realizada con PHP Nativo (Eso significa el PHP_ en el titulo) que será de utilidad para algunos usuarios y será enfocado en su totalidad para agregar al conjunto de aportes a mi portafolio personal. 

Fue realizado bajo la siguiente arquitectura:

* Servidor Apache (Wampserver 3.1.3)
* PHP Versión 7.0.29
* MySQL versión 5.7.21

### Pasos previos

* Deberás crear una base de datos llamada __login_api__ con un cotejamiento __utf8_general_ci__, ir a la sección SQL e importar el archivo __login_api.sql__ que se sitúa en la carpeta __query__

### Cosas a considerar

* La API se comunica a través del protocolo __HTTP__ y en específico peticiones __POST__ para enviar los parámetros sin que estos viajen por la URL si no en la cabecera.
* Las respuestas __positivas__ de las peticiones son en formato __JSON__ con los siguientes paráametros:
    * __uuid__
    * __name__
    * __email__
    * __created_at__
    * __updated_at__
    * __login_status__
*Las respuestas __negativas__ de las peticiones son en formato __JSON__ con los siguientes parámetros:
    * __error__
    * __error_msg__

## English

This small exercise consists of a small API Rest made with PHP Native (That means the PHP_ in the title) that will be useful for some users and will be focused in its entirety to add to the set of contributions to my personal portfolio.

It was made under the following architecture:

* Apache Server (Wampserver 3.1.3)
* PHP Version 7.0.29
* MySQL versión 5.7.21

### Previous steps

* You must create a database called __login_api__ with a collation __utf8_general_ci__, go to the SQL section and import the file __login_api.sql__ that is placed in the folder __query__

### Things to know

* The API communicates through the __HTTP__ protocol and in specific __POST__ requests to send the parameters without them traveling through the URL if not in the header.
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