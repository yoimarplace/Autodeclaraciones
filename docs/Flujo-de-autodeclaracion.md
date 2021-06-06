# Flujo-de-autodeclaracion

1.	Para generar la declaración se debe consumir el metodo **income-request-aio** enviando la trama de información de la empresa y el declarante junto con la URL de retorno en el objeto: returnURL.

2.  Placetopay responde con el identificador: requestID y el redirecTO.

3.	Guardar el requestID en relación al usuario.

4.  Redireccionar al usuario al redirecTO.

5.	Placetopay crea o actualiza los datos de la empresa y los datos del usuario en caso de que existan.

6.	Placetopay genera el formato PDF para proceder con las firmas virtuales.

7.	El representante legal y ( el revisor fiscal ) autorizan con su usuario y contraseña para que la declaración pueda ser pagada.

8.	Al ser aprobada el usuario puede proceder con el pago, el cual es redireccionado a la interfaz de Webcheckout para realizar el proceso transaccional.

9.	Al finalizar el pago el sistema le muestra un comprobante de que la declaración ha sido pagada con el cello de certificación.

10.  El usuario regresa al comercio con la URL proporcionada por el comercio.

11.  Para consultar el estado de la declaración se debe consumir el metodo information-request enviando el requestID

12. Para descargar el pdf se debe consumir el metodo income-pdf enviando el requestID y el locale.


[Imagen de flujo](https://lucid.app/publicSegments/view/890a7af8-73bd-49f1-a91d-511cca52a1b4/image.pdf)

