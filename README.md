# [PHP_] - APILoginRegister

## Español

Éste pequeño ejercicio consiste en una pequeña API Rest realizada con PHP Nativo (Eso significa el PHP_ en el titulo) que será de utilidad para algunos usuarios y será enfocado en su totalidad para agregar al conjunto de aportes a mi portafolio personal. 

Fue realizado bajo la siguiente arquitectura:

* Servidor Apache (Wampserver 3.1.3)
* PHP Versión 7.0.29
* MySQL versión 5.7.21

### Pasos previos

* Deberás crear una base de datos llamada __login_api__ con un cotejamiento __utf8_general_ci__, ir a la sección SQL e improtar el archivo __login_api.sql__ que se sitúa en la carpeta __query__

### Cosas a considerar

* La API se comunica a través del protocolo HTTP y en específico peticiones __POST__ para enviar los parámetros sin que estos viajen por la URL si no en la cabecera.
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