# T-picos-de-telem-tica

¿CUAL ES LA PROBLEMÁTICA QUE QUIERE RESOLVER?

Para este proyecto se desarrolló una aplicación IoT web que permite el registro periódico de sensores dentro de una empresa, la problemática que se intenta resolver es la gran dificultad y consumo de tiempo que presenta el registro manual de los sensores, con el propósito de mejorar la productividad de la organización, se desarrolló esta aplicación que permitirá el registro periódico automatizado.

¿CUALES SON LOS REQUISITOS FUNCIONALES DE LA APP?
Requisitos Funcionales del Sistema
El sistema debe permitir registrar los datos proporcionados por sensores de temperatura, humedad y GPS desde un dispositivo arduino.
El sistema debe permitir a los usuarios visualizar los datos proporcionados por los sensores de temperatura, humedad y GPS desde un dispositivo arduino.
El sistema debe permitir a los usuarios realizar un registro manual de los datos proporcionados por los sensores de temperatura, humedad y GPS desde un dispositivo arduino. .
El sistema debe permitir a los usuarios editar y eliminar los datos que considere pertinentes.
El sistema debe permitir usuarios ingresar al sistema a través de un login.
El sistema debe almacenar el e-mail y contraseña de los usuarios.

¿CUALES SON LOS REQUISITOS NO FUNCIONALES DE LA APP?

El sistema debe registrar menos de 2 fallas/hora, con un entrenamiento base de 2 horas(Eficiencia)
Métrica: Fallas/hora.
El sistema debe ajustarse a las relaciones de aspecto(16:9, 17:9, 18:9) y resoluciones(480p-4K)(Portabilidad)
Métrica: Relación y resolución.
El sistema debe ser compatible con la última versión de Google Chrome, Mozilla Firefox, Opera. Debido a que estos son los navegadores web más comunes.(Portabilidad)
El sistema debe estar disponible el 99% (712.8 horas) del tiempo mensual, el 1% restante se empleará para mantenimiento.(Disponibilidad) Métrica:Horas


¿QUÉ TECNOLOGÍA DE DESARROLLO UTILIZÓ?

En el backend implementé node.js con mongo.db, para el frontend utilicé Angular. MEAN


¿CUALES SON Y CUAL ES LA ESPECIFICACIÓN DE LOS SERVICIOS API REST DEL BACKEND?
Las rutas implementadas en el backend de la aplicación fueron user.js y sensor.js, que permiten controlar las funcionalidades del Login y gestión de los sensores respectivamente. 
Se crearon 4 rutas para los sensores(sensor.js), todas se acceden mediante la dirección raíz, por los métodos put, get post y delete.
El método get obtiene las medidas de los sensores, el método post permite crear medidas de los sensores(en caso de que un usuario quiera ingresar los datos obtenidos por los sensores manualmente), el método put permite actualizar y editar las medidas y el método delete eliminarlas, se agregaron estas funcionalidades pensando en una sesión de administrador que esté autorizado para realizar estos cambios.
Se crearon tres rutas para los usuarios
¿CÓMO REALIZÓ LA AUTENTICACIÓN DE LOS SERVICIOS API REST?
 autenticación mediante tokens, que genera token para cada usuario con jwt-simple

¿CUALES SON LAS PRINCIPALES DIFICULTADES QUE TUVO AL DESARROLLAR EL PROYECTO?
7.1 POR DESCONOCIMIENTO DE LA TECNOLOGÍA?

7.2 ¿QUÉ CONCEPTOS O FUNDAMENTOS NO SABE PARA PODER DESARROLLAR ESTE PROYECTO?
antes de la realización del proyecto, no sabía como utilizar el framework angular, y la utilización de tokens para la autenticación
7.3 ¿QUÉ HABILIDADES DE DESARROLLO LE FALTAN PARA PODER TERMINAR EL PROYECTO?
Mejorar habilidades en la utilización del framework angular.
7.4 ¿QUÉ OTRAS COSAS LE FALTÓ PARA PODER DESARROLLAR EL PROYECTO 1?
Presenté dificultades en la utilización de tokens para realizar la autenticación de los usuarios, no logré integrar los tokens generados en el backend con el frontend.

¿CUALES FUERON LOS PRINCIPALES APRENDIZAJES DEL PROYECTO 1?
Considero que uno de los principales aprendizajes que obtuve con la realización de este proyecto fueron los conocimientos adquiridos en el framework angular, logré identificar a cabalidad las capas del patrón mvc para cada uno de los frameworks implementados, tanto en el backend como el frontend.

